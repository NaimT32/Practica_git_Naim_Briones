# Práctica de Git y GitHub
## Datos del estudiante

*Nombre completo:* Naim Tadeo Garcia Briones  
*Matrícula:* 2630476  
*Nombre de la práctica:* Creación y sincronización de repositorios con Git y GitHub

---

## Objetivo de la práctica

El objetivo de esta práctica fue aprender a crear y administrar un repositorio local utilizando Git, vincularlo con un repositorio remoto en GitHub y comprobar la sincronización de información en ambos sentidos.

---

## Descripción del procedimiento realizado

Primero se creó una carpeta para la práctica y se abrió PowerShell dentro de ella. Posteriormente se inicializó un repositorio local utilizando Git.

Después se configuró la rama principal con el nombre main y se crearon los archivos README.md y datos.txt.

Una vez creados los archivos, se verificó el estado del repositorio y se agregaron los archivos al área de preparación. Posteriormente se realizó el primer commit para guardar los cambios en el repositorio local.

Después se creó un repositorio público en GitHub con el mismo nombre de la práctica. El repositorio remoto se dejó vacío para poder enviar los archivos desde el repositorio local.

Se vinculó el repositorio local con GitHub mediante la configuración de un repositorio remoto llamado origin. Finalmente, se realizó un git push para enviar los archivos y el historial de commits desde el repositorio local hacia GitHub.

---

## Comandos de Git utilizados

### git init

Inicializa un nuevo repositorio de Git dentro de la carpeta actual.

### git branch -M main

Establece el nombre de la rama principal como main.

### git status

Permite consultar el estado actual del repositorio y conocer qué archivos han sido modificados, cuáles están preparados para realizar un commit y cuáles todavía no están siendo rastreados.

### git add .

Agrega todos los archivos y cambios disponibles al área de preparación.
### git commit -m "Primer commit"

Crea un commit con los cambios que se encontraban en el área de preparación.

### git remote add origin URL_DEL_REPOSITORIO

Vincula el repositorio local con el repositorio remoto de GitHub. origin es el nombre utilizado para identificar el repositorio remoto.

### git remote -v

Permite comprobar la dirección del repositorio remoto que está vinculado con el repositorio local.

### git push -u origin main

Envía los commits y archivos del repositorio local hacia la rama main del repositorio remoto en GitHub. Con esto se realizó la primera sincronización de Local → GitHub.

### git pull origin main

Descarga los cambios que existen en el repositorio remoto de GitHub y los integra en el repositorio local. Este comando permitió comprobar la sincronización de GitHub → Local.

### git push

Envía los nuevos commits realizados en el repositorio local hacia GitHub después de que el repositorio ya se encuentra vinculado.

---

## Creación del repositorio local

El repositorio local se creó dentro de la carpeta de la práctica utilizando el comando git init.

Después se configuró la rama principal como main. Se crearon los archivos necesarios para la práctica y se utilizó git status para comprobar el estado de los archivos.

Posteriormente se utilizó git add . para agregar los archivos al Staging Area y finalmente se realizó el primer commit con el comando:

git commit -m "Primer commit"

De esta manera, los archivos quedaron registrados dentro del repositorio local.

---

## Vinculación del repositorio local con GitHub

Después de crear el repositorio público en GitHub, se utilizó el comando git remote add origin para establecer la conexión entre el repositorio local y el repositorio remoto.

La conexión se comprobó mediante:

git remote -v

Una vez comprobada la conexión, se utilizó:

git push -u origin main

para enviar el contenido del repositorio local a GitHub.

---

## Sincronización Local → GitHub

La primera sincronización se realizó enviando los archivos y el primer commit desde el repositorio local hacia GitHub mediante:

git push -u origin main

Posteriormente se realizaron modificaciones en el archivo datos.txt desde el repositorio local. Estos cambios fueron agregados con git add ., registrados mediante un nuevo commit y enviados nuevamente a GitHub utilizando git push.

Esto permitió comprobar que los cambios realizados en la computadora podían actualizar correctamente el repositorio remoto.

---

## Sincronización GitHub → Local

Para comprobar el flujo contrario, se modificó directamente el archivo datos.txt desde la página de GitHub.

Se agregó la línea:

> Este archivo fue modificado desde GitHub.

Después de guardar el cambio mediante un commit en GitHub, se regresó al repositorio local y se utilizó:

git pull origin main

Este comando descargó los cambios realizados en GitHub y los incorporó al repositorio local.

Al abrir nuevamente el archivo datos.txt en la computadora se pudo comprobar que el cambio realizado desde GitHub también estaba presente localmente.

---

## Cambios realizados desde el repositorio local

Después de comprobar la sincronización desde GitHub hacia la computadora, se modificó nuevamente el archivo datos.txt desde el repositorio local.

Se agregó la línea:

> Este archivo fue modificado desde el repositorio local.

Después se verificó el estado del repositorio con git status, se agregaron los cambios con git add ., se creó un nuevo commit y finalmente se utilizó git push para enviar la modificación a GitHub.

De esta manera se comprobó nuevamente el flujo:

*Repositorio Local → GitHub*

---

## Archivos contenidos en el repositorio

### README.md

Es el archivo de documentación de la práctica. Contiene información sobre el estudiante, el objetivo, el procedimiento realizado, los comandos utilizados y la explicación de la sincronización entre Git y GitHub.

### datos.txt

Es el archivo utilizado para realizar las modificaciones durante la práctica. En él se realizaron cambios tanto desde GitHub como desde el repositorio local para comprobar que la información pudiera sincronizarse correctamente.

---

## Historial de commits

Durante la práctica se realizaron varios commits para registrar los diferentes cambios realizados.

Entre ellos se encuentra el commit inicial:

Primer commit

También se realizó un commit desde GitHub al modificar el archivo datos.txt y posteriormente otro commit desde el repositorio local:

Actualización desde repositorio local

El historial de commits permite comprobar los diferentes cambios realizados durante la práctica.

---

## Conclusión

Con esta práctica aprendí a utilizar Git para controlar las versiones de un proyecto y a trabajar con un repositorio remoto en GitHub. Comprendí la función del Working Directory, el Staging Area y el repositorio local, así como la importancia de los commits para guardar los cambios realizados. También aprendí a vincular un repositorio local con GitHub y a utilizar git push para enviar cambios al repositorio remoto y git pull para obtener los cambios realizados desde GitHub. La práctica permitió comprobar de manera práctica que un proyecto puede mantenerse sincronizado entre una computadora y GitHub, trabajando en ambos sentidos. En conclusión, Git y GitHub son herramientas útiles para llevar un control de las versiones de un proyecto, mantener un historial de cambios y facilitar el trabajo con repositorios locales y remotos.