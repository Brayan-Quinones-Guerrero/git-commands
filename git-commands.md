# GIT Commands


## Clonación de repositorios
### `git clone <url-repositorio>`
- **Descripción:** Clona un repositorio remoto en tu máquina local.
- **Ejemplo de uso:**
  ```bash
  git clone https://github.com/usuario/proyecto.git
  ```


## Inicialización del repositorio
### `git init`
- **Descripción:** Inicializa un nuevo repositorio Git en el directorio actual.
- **Ejemplo de uso:**
  ```bash
  git init
  ```


## Manejo de archivos
### `git add <archivo>`
- **Descripción:** Agrega archivos al área de preparación (staging area) para ser incluidos en el próximo commit.
- **Condición:** El archivo debe existir en el directorio del proyecto.
- **Ejemplo de uso:**
  ```bash
  git add archivo.txt
  ```

### `git add .`
- **Descripción:** Agrega todos los archivos modificados y nuevos del *directorio actual* al área de preparación.
- **Ejemplo de uso:**
  ```bash
  git add .
  ```

### `git rm --cached <archivo>`
- **Descripción:** Elimina un archivo del área de preparación sin eliminarlo del sistema de archivos. El archivo permanecerá en tu directorio de trabajo, pero no será incluido en el próximo commit.
- **Condición:** El archivo debe estar en el área de preparación.
- **Ejemplo de uso:**
  ```bash
  git rm --cached archivo.txt
  ```

### `git rm --cached -f <archivo>`
- **Descripción:** Fuerza la eliminación de un archivo del área de preparación.
- **Ejemplo de uso:**
  ```bash
  git rm --cached -f archivo.txt
  ```
  
### `git restore <archivo>`
- **Descripción:** Restaura un archivo al estado que tenía en el último commit, descartando cualquier cambio no confirmado.
- **Ejemplo de uso:**
  ```bash
  git restore archivo.txt
  ```

### `git checkout <archivo>`
- **Descripción:** Restaura un archivo al estado que tenía en el último commit, descartando cualquier cambio no confirmado en dicho archivo.
- **Uso:**
  ```bash
  git checkout archivo.txt
  ```

### `git checkout -- .`
- **Descripción:** Restaura todos los archivos modificados al estado que tenían en el último commit, descartando cualquier cambio no confirmado en el área de trabajo.
- **Ejemplo de uso:**
  ```bash
  git checkout -- .
  ```

### `git stash`
- **Descripción:** Guarda temporalmente los cambios no confirmados para limpiar el área de trabajo sin necesidad de hacer un commit. Se utiliza cuando necesitas cambiar de rama o hacer un git pull sin perder los cambios actuales.
- **Ejemplo de uso:**
  ```bash
  git stash
  ```

### `git stash pop`
- **Descripción:** Aplica los cambios más recientes guardados con `git stash` y los elimina de la lista de stashes. Esto te permite recuperar los cambios que habías guardado temporalmente.
- **Ejemplo de uso:**
  ```bash
  git stash pop
  ```


## Estado del repositorio
### `git status`
- **Descripción:** Muestra el estado del repositorio, indicando archivos modificados, agregados y no rastreados.
- **Ejemplo de uso:**
  ```bash
  git status
  ```

### `git status -s`
- **Descripción:** Muestra el estado del repositorio de manera abreviada.
- **Ejemplo de uso:**
  ```bash
  git status -s
  ```


## Confirmación de cambios
### `git commit -m "message"`
- **Descripción:** Confirma los cambios agregados al área de preparación en el repositorio, con un mensaje de confirmación.
- **Ejemplo de uso:**
  ```bash
  git commit -m "Primer commit"
  ```

### `git commit -am "message"`
- **Descripción:** Añade todos los archivos *modificados* (no los nuevos) al área de preparación y los confirma con un mensaje, todo en un solo paso.
- **Condición:** Este comando no agrega archivos nuevos al área de preparación, solo los modificados.
- **Ejemplo de uso:**
  ```bash
  git commit -am "Modificaciones rápidas"
  ```


## Historial del repositorio
### `git log`
- **Descripción:** Muestra el historial de commits en el repositorio, con detalles como el autor, fecha y 
mensaje del commit.
- **Ejemplo de uso:**
  ```bash
  git log
  ```

### `git log --oneline`
- **Descripción:** Muestra el historial de commits en un formato más compacto, con un resumen de una sola linea
por commit.
- **Ejemplo de uso:**
  ```bash
  git log --oneline
  ```

## Comparación de cambios
### `git diff <archivo>`
- **Descipción:** Muestra las diferencias entre el archivo actual y la última versión confirmada en el repositorio.
- **Ejemplo de uso:**
  ```bash
  git diff archivo.txt
  ```


## Control de versiones
### `git checkout <hash>`
- **Descripción:** Cambia a una versión especificada del proyecto utilizando el hash del commit.
- **Ejemplo de uso:**
  ```bash
  git checkout a1b2c3d
  ```

  
## Manejo de ramas
### `git checkout -b <nombre-rama>`
- **Descripción:** Crea una nueva rama y cambia a ella.
- **Ejemplo de uso:**
  ```bash
  git checkout -b develop
  ```

### `git branch <nombre-rama>`
- **Descripción:** Crea una nueva rama sin cambiar a ella.
- **Ejemplo de uso:**
  ```bash
  git branch develop
  ```

### `git merge <nombre-rama>`
- **Descripción:** Fusiona la rama especificada en la rama actual.
- **Ejemplo de uso:**
  ```bash
  git merge develop
  ```

### `git branch -d <nombre-rama>`
- **Descripción:** Elimina una rama local de forma segura (si ya se ha fusionado).
- **Condición:** Debes estar en una rama diferente a la que deseas eliminar. La rama no puede estar activa y debe haberse fusionado previamente.
- **Ejemplo de uso:**
  ```bash
  git branch -d vieja-rama
  ```

### `git branch -D <nombre-rama>`
- **Descripción:** Fuerza la eliminación de una rama local, incluso si no ha sido fusionada.
- **Condición:** Debes estar en una rama diferente a la que deseas eliminar. Este comando debe usarse con precaución, ya que puede resultar en la pérdida de trabajo no fusionado.
- **Ejemplo de uso:**
  ```bash
  git branch -D vieja-rama
  ```

### `git checkout <nombre-rama>`
- **Descripción:** Cambia de la rama actual a la rama especificada.
- **Condición:** La rama especificada debe existir localmente. Si tienes cambios sin confirmar, debes confirmarlos o guardarlos antes de cambiar de rama.
- **Ejemplo de uso:**
  ```bash
  git checkout main
  ```

### `git branch`
- **Descripción:** Muestra la lista de ramas existentes en el repositorio, con un asterisco indicando la rama activa.
- **Ejemplo de uso:**
  ```bash
  git branch
  ```


## Resolución de conflictos
### Conflictos de fusión
- **Descripción:** Los conflictos de fusión ocurren cuando Git no puede fusionar automáticamente los cambios debido a modificaciones conflictivas en los archivos. En estos casos, Git marca los conflictos en los archivos afectados.
- **Proceso de resolución:**
  1. Revisa los archivos en conflicto marcados por Git (puedes usar `git status` para ver la lista).
  2. Edita manualmente los archivos para resolver los conflictos. Git marcará las secciones conflictivas con `<<<<<<<`, `=======`, y `>>>>>>>`.
  3. Una vez resueltos los conflictos, agrega los archivos resueltos al área de preparación con `git add`.
  4. Completa la fusión confirmando los cambios con `git commit`.
- **Comandos útiles:**
  ```bash
  git status          # Verifica los archivos en conflicto
  git add archivo.txt # Marca un archivo resuelto
  git commit          # Confirma la resolución de conflictos
  ```


## Sincronización con repositorios remotos
### `git fetch`
- **Descripción:** Descarga los cambios de un repositorio remoto, actualizando las referencias de las ramas remotas en tu repositorio local, pero sin fusionarlos con la rama de trabajo actual. Es útil para revisar los cambios antes de hacer una fusión.
- **Ejemplo de uso:**
  ```bash
  git fetch origin
  ```

### `git pull`
- **Descripción:** Descarga y fusiona automáticamente los cambios del repositorio remoto en la rama actual. Este comando es equivalente a ejecutar `git fetch` seguido de `git merge`. Puede causar conflictos si hay cambios conflictivos entre la rama remota y tu rama local.
- **Ejemplo de uso:**
  ```bash
  git pull origin main
  ```

### `git push`
- **Descripción:** Envía los commits locales al repositorio remoto.
- **Ejemplo de uso:**
  ```bash
  git push origin main
  ```