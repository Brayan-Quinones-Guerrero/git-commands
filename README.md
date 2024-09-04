# Documentación de Comandos de Git

Este repositorio contiene una documentación organizada de los comandos más utilizados en Git, dividida en secciones para facilitar su uso durante el desarrollo de proyectos. Esta documentación está diseñada para ser una guía rápida para los comandos más comunes que se emplean en el flujo de trabajo diario con Git.

## Estructura de la Documentación

Cada sección cubre un conjunto específico de comandos relacionados con una tarea en Git. A continuación, se describen brevemente las secciones incluidas:

### 1. Repository Commands
Esta sección incluye comandos relacionados con la clonación e inicialización de repositorios:

- `git clone`: Clona un repositorio remoto en tu máquina local.
- `git init`: Inicializa un nuevo repositorio en el directorio actual.

### 2. File Commands
Aquí se encuentran comandos para agregar y eliminar archivos del área de preparación (staging area):

- `git add`: Añade archivos al área de preparación.
- `git rm --cached`: Elimina un archivo del área de preparación sin eliminarlo del directorio de trabajo.
- `git restore`: Restaura archivos al último commit.

### 3. Status Commands
Comandos para revisar el estado del repositorio y los archivos:

- `git status`: Muestra el estado de los archivos en el repositorio.
- `git status -s`: Muestra el estado de los archivos en un formato abreviado.

### 4. Commit Commands
Comandos para confirmar los cambios en el repositorio:

- `git commit`: Confirma los cambios en el área de preparación con un mensaje descriptivo.
- `git commit -am`: Añade y confirma todos los archivos modificados en un solo paso.

### 5. History Commands
Comandos para revisar el historial de cambios en el repositorio:

- `git log`: Muestra el historial de commits.
- `git diff`: Compara los cambios en los archivos.

### 6. Branch Commands
Comandos para la gestión de ramas en el repositorio:

- `git branch`: Crea, lista o elimina ramas.
- `git checkout`: Cambia de una rama a otra o crea una nueva rama.

### 7. Conflict Resolution
Explicación sobre cómo manejar los conflictos de fusión en Git:

- Pasos para resolver conflictos manualmente.
- Comandos útiles para gestionar conflictos.

### 8. Remote Commands
Comandos para interactuar con repositorios remotos:

- `git fetch`: Descarga cambios del repositorio remoto sin fusionarlos.
- `git pull`: Descarga y fusiona cambios del repositorio remoto en la rama actual.
- `git push`: Envía los commits locales al repositorio remoto.

## Contribución

Si deseas contribuir a la mejora de esta documentación, puedes crear una nueva rama basada en el siguiente formato: `feature/<descripción>`, realizar los cambios y enviar un pull request.

---

Esta documentación está enfocada en ser clara y práctica, proporcionando ejemplos y explicaciones sobre las condiciones de uso de cada comando.

¡Espero que te sea útil para trabajar de manera eficiente con Git!