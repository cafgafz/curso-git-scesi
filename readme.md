CURSO DE GIT POSTULANTES SCESI UMSS 2024

En este README encontraras todo lo avanzado durante estas clases, junto con informacion adicional sobre GIT.

***<u>CLASE N#1</u>***

QUE ES GIT?
Es el sistema controlador de versiones mas famoso del mundo, un proyecto de codigo abierto originalmente esarollado por LINUS TORVALDS, el famoso creador del kernel del sistema operativo LINUX

EL OBJETIVO DE GIT:

Tener un entorno para poder realizar proyectos individuales y en colaboracion donde las persona puedan trabajar y hacer aportes sin perder el tiempo(opinion personal).

**COMANDOS DE BASH SOBRE LA TERMINAL BASADA EL LINUX**

- **pwd** (directorio en el que actualmente te encuentras)
- **cd** (change directory)
- **ls** (listar los archivos que tienes en el directorio que tienes) **al** (argumento para mostrar los archivos ocultos)
- **ctrl + L** (Limpiar la terminal)
- **mkdir directoryName** (crear una carpeta)
- **touch fileName.extension** (crear archivos vacíos)
- **cat fileName.extension** (ver rápidamente el contenido de un archivo en consola)
- **history** (muestra un listado de todos los comandos empleados en la consola)
- **! + comandNum** (vuelve a ejecutar el comando de la lista mostrado en history)
- **rm fileName.extension** (borra el documento)
- **anyCommand** -**help** (explica para qué sirve ese comando)
- **esc + shift + zz** (Salir del editor de vimm)
- **alias aliasname=”the command that you want to save with an alias”** (guardar comandos largos en un alias para no acordarse todo el código largo)



CONCEPTOS NECESARIOS PARA ENTENDER GIT

STAGED:

En Git, "staging" se refiere al proceso de preparar cambios en archivos para que sean incluidos en el próximo commit, entonces el staged es el lugar dentro de la memoria RAM donde los archivos se encuentran trackeados(que se les hace un seguimiento)

HEAD:

Es un puntero especial que hace referencia al último commit en la rama actual. En otras palabras, es un puntero móvil que apunta al commit actualmente activo en tu repositorio.

RAMAS: 

Las ramas son una forma de trabajar en diferentes versiones de un repositorio al mismo tiempo, son basicamente una instantanea de la division del estado del codigo. Cada repositorio de Git tiene al menos una rama, que normalmente se llama "master" (o "main" en algunas configuraciones más recientes), que es la rama por defecto cuando se crea un repositorio.

COMANDOS BASICOS DE GIT...

"git init"

Este comando se usa para inicializar git y crear el repositorio de manera local dentro de una carpera o directorio ya existente.
"git add"

Este comando se usa para a añadir archivos al staged, se puede seleccionar el archivo a trakear o hacer un add de toda la carpeta(git add .).

"git status"

Se utiliza en Git para mostrar el estado actual de tu repositorio. Proporciona información sobre qué archivos han sido modificados, qué archivos están en el área de staging (preparados para el próximo commit) y qué archivos no están siendo trackeados por Git.

"git commit"

 Este comando nos sirve para mandar los archivos que tenemos en nuestro staged al repositorio local anteriormente creado.

"git log"

El comando git log nos muestra el historial de commits realizados desde la creacion del repositorio.

<u>***<mark>CLASE N#2</mark>***</u>

COMANDOS PARA CREACION DE RAMAS:

"git branch"

Este comando crea una rama.

"git switch"

Para moverte entre ramas.

"git checkout"

Este es el comando que yo utilizaba para moverme entre ramas.s
