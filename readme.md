CURSO DE GIT POSTULANTES SCESI UMSS 2024

En este README encontraras todo lo avanzado durante estas clases, junto con informacion adicional sobre GIT.



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

MERGE:

Se refiere a la fusion o incorporacion de cambios traidos desde otra rama a la rama actual o donde esta el puntero HEAD.



***<u>CLASE N#1</u>***

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

BRANCH

RAMAS:

Las ramas son una forma de trabajar en diferentes versiones de un repositorio al mismo tiempo, son basicamente una instantanea de la division del estado del codigo. Cada repositorio de Git tiene al menos una rama, que normalmente se llama "master" (o "main" en algunas configuraciones más recientes), que es la rama por defecto cuando se crea un repositorio.

MERGE:

Se refiere a la fusion o incorporacion de cambios traidos desde otra rama a la rama actual o donde esta el puntero HEAD.

**COMANDOS PARA CREACION DE RAMAS:**

"git branch"

Este comando crea una rama.

"git switch"

Para moverte entre ramas.

"git checkout"

Este es el comando que yo utilizaba para moverme entre ramas.

"git branch -d"

Comando para eliminar una rama.

"git branch -a"

Para ver las ramas locales y remotas.





**COMANDOS SOBRE FUSION DE RAMAS**

"git merge"

Comando para añadir los cambios de otra rama a la rama actual(donde esta el HEAD).

"git merge --edit"

Abre el editor antes de hcaer commit.

"git merge --no-commit"

Evita que haga commit automaticamente.

"git diff"

Este comando nos sirve para ver las diferencias entre achivos, en la fusion o merge o tambien para casos generales cuando queremos saber que cambios se han realizado sobre un archivo.

 

***<u><mark>CLASE N#3</mark></u>***

**REPOSITORIOS REMOTOS**

Un repositorio remoto en Git es una versión de tu proyecto que esta alojada en un servidor en línea o en otro lugar accesible a través de Internet. Este repositorio remoto puede contener una copia completa del historial de tu proyecto, así como las ramas y los commits que has realizado.

**GITHUB**

GitHub es una plataforma de desarrollo colaborativo para alojar proyectos utilizando el sistema de control de versiones Git. Es uno de los servicios de alojamiento de repositorios remotos más populares y ofrece diversas herramientas para facilitar la colaboración en proyectos de software.

Diferencia entre Git y GitHub

- **Git** es el sistema de control de versiones.

- **GitHub** es un servicio de alojamiento en la nube de código fuente.

**COMANDOS PARA REPOSITORIOS REMOTOS**

"git remote add origin URLrepositorio"

Comando para añadir un repositorio remoto(github, gitlab, ect)

"git remote set-url remoteName URLrepositorio"

Comando para editar url de un repositorio.

"git remote remove"

Comando para borrar un repositorio remoto.

"git remote -v"

Para ver todos los repositorios remotos mas urls que estan en nuestro local.



**PULL AND PUSH**



"git pull nombreRepoRemoto ramalocal"

Para traer todos los cambios del repositorio remoto.

"git pull remoteRepositoryName localBranchName --allow-unrelated-histories"

Para forzar traer todos los cambios del remoto.

"git push "

Para pushear o subir los cambios al repositorio remoto.

"git push -f "

Para forzar el subir los cambios o pushear al remoto.

"git clone urlrepo"

Para clonar un repositorio remoto en tu local.

CREACION DE UNA RAMA REMOTA

"git switch -c"

Para crear una rama en el local y movernos automaticamente a ella.

"git push origin website"

Mandamos la rama local al remoto, ten en cuenta que primero siempre debes crear la rama de lo contrario te dara error.

"git fetch"

Actualiza la informacion de la rama remota en la local, para poder traer una rama del remoto al local, primero git fetch y luego nos cambiamos a la rama para poder tenerla en el local.

"git remote prune origin"
Eliminar ramas remotas de nuestro local(actualizar que ya no existen).





<mark>***<u>CLASE#4</u>***</mark>

**PULL REQUEST**

Abreviada PR, es una solicitud de cambios enviados al repositorio original.

HACER UNA BUENA PULL REQUEST

1.- Enfocar el codigo en una sola cosa.

2.- Explicar la pull request un video o grabar pantalla.





***<u><mark>CLASE N#5</mark></u>***



GIT FLOW

Es un modelo de ramificación para Git que se centra en cómo se gestionan las ramas en un proyecto Git. Fue popularizado por Vincent Driessen en un artículo de 2010 y desde entonces ha sido adoptado por muchos equipos de desarrollo de software debido a su enfoque estructurado y su capacidad para gestionar proyectos de forma eficiente.

Feature: Caracteristicas nuevas para el proyecto.

Release: Cambios de ultimo momento.

Hotfix: Parches o arreglar bugs pequenios.





GITHUB FLOW

Rama main y cualquier otra rama que quiera ser integrada por medio de PR.

Es la alternativa mas simple a GIT FLOW. Tiene menos liturgias, es mas facil de entender y favorece los despliegues continuos de tu proyecto.





TRUNK BASED DEVELOPMENT

    Solo la rama main y ramas auxiliares efimeras que quiera ser integrada por medio de una pull request.

Es util si contamos con un buen sistema CI/CD. En esta estrategia se prioriza hcaer commits directamente a la rama principal, en el caso de necesitar ramas se hacen pequenias PR y que duren poco tiempo para ser integradas lo antes posible.







SHIP / SHOW / ASK

1.- Ship: Se fusiona en la rama principal sin revision.

2.- Show: Abre una peticion de cambios para que sean revisados por CI pero se fusiona inmediatamente.

3.- Ask: Abre una PR para discutir los cambios antes de fusionarlos \.

Algunas de las reglas :

Tenemos un buen sistema CI/CD.

Confiamos en el equipo y tenmos buenas practicas de desarrollo.

Las revisiones de codigo no son requerimientos.

Las ramas son lo mas pequenias posibles.





<mark><u>***CLASE N#6***</u></mark>



CADA CUANTO HACER UN COMMIT?

 La respuesta es a menudo.

Es mejor hacer commits pequenios, agrupando pequenias mejoras o acciones, que un commit con todo lo que se quiere hacer.

Hacer commits a menudo no significa hacerlos sin sentido.

BUENAS PRACTICAS SOBRE COMMITS

- Usar el verbo imperativo(add, change, fix, remove)
- No usar puntos suspensivos ni final en los mensajes del commit.
- Usa como maximo 50 caracteres e tu mensaje de commit.
- Pon todo el contexto que sea necesario en el mensaje.
- Usa prefijos semanticos(feat, fix, perf, build, ci, docs, refactor, style, test, etc)

 

ESCRIBIR UN BUEN NOMBRE DE RAMA

- Se conciente al nombrar tus ramas
- Usa el nombre de la accion que se realiza en la rama
- Use los IDs de JIRA o el sistema de tickets que uses





***<u><mark>CLASE N#7</mark></u>***



EN QUE CASOS DESHACEMOS CAMBIOS?

- Dejo de funcionar el proyecto
- Queremos recuperar una parte del cdigo que eliminamos
- Queremos recuperar archivos que eliminamos
  
  
  

COMANDOS DESTRUCTIVOS Y NO DESTRUCTIVOS

Los comandos destructivos afectan al historial de commits realizados, por contrario los nos destructivos trabajan en base al historial sin afectarlos.

"git reset"

Posee 2 opciones:

- <u>soft </u>: Mantiene los cambios que ocurrieron antes de hacer commit, mantiene los archivos que estaban siendo trackeados(staged).
- <u>hard</u>: descarta los cambios (es el mas usado).

"git revert"

Revierte los cambios que un commit introdujo y crea un commit nuevo con los cambios revertidos.

"git checkout""

Nos permite recuperar codigo especifico de commits.

"git checkout HASH filename"

Nos permite traer una version anterior de un archivo a nuestra rama actual sin afectar demas archivos.





<u><mark>***CLASE N#8***</mark></u>





HOOKS

Son eventos que se realizan antes o despues de ciertos comandos, podria verse como en base de datos TRIGGERS para mayor entendimiento.

Son scripts personalizables que se ejecutan automáticamente en respuesta a ciertos eventos en un repositorio Git. Estos scripts permiten realizar acciones específicas antes o después de que ocurran eventos como hacer un commit, fusionar ramas, recibir cambios desde un repositorio remoto, entre otros.

Los hooks del lado del cliente solo afectan al repositorio local que los contiene.

1. **pre-commit**: Se ejecuta justo antes de realizar un commit. Puede utilizarse para realizar verificaciones de código, pruebas automáticas u otras acciones para garantizar que el commit cumpla con ciertos estándares.

2. **post-commit**: Se ejecuta después de realizar un commit. Puede utilizarse para notificar a los desarrolladores sobre el commit, actualizar la documentación u otras acciones posteriores al commit.

3. **pre-push**: Se ejecuta antes de enviar cambios locales a un repositorio remoto. Puede utilizarse para realizar pruebas finales o asegurarse de que los cambios locales no rompan la integración con el repositorio remoto.

4. **post-merge**: Se ejecuta después de que se haya fusionado una rama en otra. Puede utilizarse para realizar acciones específicas después de una fusión, como actualizar dependencias o ejecutar migraciones de base de datos.





COMO CREAR MI PRIMER HOOK

Para crear un propio hook solo tienes que crear un archivo nombre-del-hook en la carpeta .git/hooks y  en el poner el codigo que quieres que se ejecute.

Puedes usar todo tipo de interpretes de lenguaje de programacion como bash, node, python, perl, etc.



QUE ES UN ALIAS

Un alias son nombres abreviados que se le pueden dar a comados dentro de git, permiten definir una serie de comandos que puden ser usados en lugar de los nombres completos. Se usan para facilitar la escritura, agilizar el proceso y hacer del ambiente de trabajo algo mas intimo y personalizado para el usuario.

git co --> git commit

git st --> git status

"git config --global alias.nombre_alias "comando_git""

Comando para crear un alias en nuestra terminal.

"git config --unset alias.nombre_alias"

Comando para borrar un alias.





TRUCOS EN GIT





GUARDAR CAMBIOS TEMPORALMENTE

"git stash"

Es un comando en Git que se utiliza para "guardar" temporalmente los cambios locales que aún no han sido comprometidos en un "stash" (oculto). Esto es útil cuando quieres cambiar de rama o hacer algo más en tu repositorio sin comprometer tus cambios actuales. Básicamente,  te permite guardar un estado de trabajo en progreso para que puedas volver a él más tarde (lo guarda en una pila).

"git stash -u"

Guardara en el stash los archivos que esten y tambien los que no esten en el staged.

"git stash pop"

Para eliminar un archivo puesto en la pila.
