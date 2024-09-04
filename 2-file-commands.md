## `git add <archivo>`
- **Descripción:** Agrega archivos al área de preparación (staging area) para ser incluidos en el próximo commit.
- **Condición:** El archivo debe existir en el directorio del proyecto.
- **Ejemplo de uso:**
  ```bash
  git add archivo.txt
  ```

## `git add .`
- **Descripción:** Agrega todos los archivos modificados y nuevos del *directorio actual* al área de preparación.
- **Ejemplo de uso:**
  ```bash
  git add .
  ```

## `git rm --cached <archivo>`
- **Descripción:** Elimina un archivo del área de preparación sin eliminarlo del sistema de archivos. El archivo permanecerá en tu directorio de trabajo, pero no será incluido en el próximo commit.
- **Condición:** El archivo debe estar en el área de preparación.
- **Ejemplo de uso:**
  ```bash
  git rm --cached archivo.txt
  ```

## `git rm --cached -f <archivo>`
- **Descripción:** Fuerza la eliminación de un archivo del área de preparación.
- **Advertencia:** Usar con precaución, ya que puede provocar la pérdida de cambios en el área de preparación.
- **Ejemplo de uso:**
  ```bash
  git rm --cached -f archivo.txt
  ```
  
## `git restore <archivo>`
- **Descripción:** Restaura un archivo al estado que tenía en el último commit, descartando cualquier cambio no confirmado. Recomendado sobre `git checkout` para restaurar archivos.
- **Ejemplo de uso:**
  ```bash
  git restore archivo.txt
  ```

## `git restore --source HEAD --staged .`
- **Descripción:** Restaura todos los archivos modificados al estado del último commit, descartando cualquier cambio no confirmado en el área de trabajo. Este comando es más moderno que `git checkout -- .` y se recomienda para restaurar el estado del repositorio.
- **Condición:** Debe haber cambios no confirmados en el área de trabajo.
- **Ejemplo de uso:**
  ```bash
  git restore --source HEAD --staged .
  ```

## `git stash`
- **Descripción:** Guarda temporalmente los cambios no confirmados para limpiar el área de trabajo sin necesidad de hacer un commit. Se utiliza cuando necesitas cambiar de rama o hacer un git pull sin perder los cambios actuales.
- **Advertencia:** Ten cuidado, ya que si no aplicas correctamente el stash, los cambios podrían perderse.
- **Ejemplo de uso:**
  ```bash
  git stash
  ```

## `git stash pop`
- **Descripción:** Aplica los cambios más recientes guardados con `git stash` y los elimina de la lista de stashes. Esto te permite recuperar los cambios que habías guardado temporalmente.
- **Ejemplo de uso:**
  ```bash
  git stash pop
  ```