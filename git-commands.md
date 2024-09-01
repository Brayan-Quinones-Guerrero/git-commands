# GIT Commands


## Inicialización del repositorio
### `git init`
- **Descripción:** Inicializa un nuevo repositorio Git en el directorio actual.
- **Uso:**
  ```bash
  git init
  ```


## Manejo de archivos
### `git add <archivo>`
- **Descripción:** Agrega archivos al área de preparación (staging area).
- **Uso:**
  ```bash
  git add <archivo>
  ```
  - **Ejemplo:**
    ```bash
    git add archivo.txt
    ```

### `git add .`
- **Descripción:** Agrega todos los archivos modificados y nuevos del *directorio actual* al área de preparación.
- **Uso:**
  ```bash
  git add .
  ```

### `git rm --cached <archivo>`
- **Descripción:** Elimina un archivo del área de preparación sin eliminarlo del sistema de archivos.
- **Uso:**
  ```bash
  git rm --cached <archivo>
  ```
  - **Ejemplo:**
    ```bash
    git rm --cached archivo.txt
    ```

### `git rm --cached -f <archivo>`
- **Descripción:** Fuerza la eliminación de un archivo del área de preparación.
- **Uso:**
  ```bash
  git rm --cached -f <archivo>
  ```
  - **Ejemplo:**
    ```bash
    git rm --cached -f archivo.txt
    ```
  
### `git restore <archivo>`
- **Descripción:** Restaura un archivo al estado que tenía en el último commit, descartando cualquier cambio no confirmado.
- **Uso:**
  ```bash
  git restore <archivo>
  ```
  - **Ejemplo:**
    ```bash
    git restore archivo.txt
    ```

### `git checkout <archivo>`
- **Descripción:** Restaura un archivo al estado que tenía en el último commit, descartando cualquier cambio no confirmado en dicho archivo.
- **Uso:**
  ```bash
  git checkout <archivo>
  ```
  - **Ejemplo:**
    ```bash
    git checkout archivo.txt
    ```

### `git checkout -- .`
- **Descripción:** Restaura todos los archivos modificados al estado que tenían en el último commit, descartando cualquier cambio no confirmado en el área de trabajo.
- **Uso:**
  ```bash
  git checkout -- .
  ```


## Estado del repositorio
### `git status`
- **Descripción:** Muestra el estado del repositorio, indicando archivos modificados, agregados y no rastreados.
- **Uso:**
  ```bash
  git status
  ```

### `git status -s`
- **Descripción:** Muestra el estado del repositorio de manera abreviada.
- **Uso:**
  ```bash
  git status -s
  ```


## Confirmación de cambios
### `git commit -m`
- **Descripción:** Confirma los cambios agregados al área de preparación en el repositorio, con un mensaje de confirmación.
- **Uso:**
  ```bash
  git commit -m "mensaje"
  ```
  - **Ejemplo:**
    ```bash
    git commit -m "Primer commit"
    ```

### `git commit -am`
- **Descripción:** Añade todos los archivos *modificados* al área de preparación y los confirma con un mensaje, todo en un solo paso.
- **Uso:**
  ```bash
  git commit -am "mensaje"
  ```
  - **Ejemplo:**
    ```bash
    git commit -am "Modificaciones rápidas"
    ```


## Historial del repositorio
### `git log`
- **Descripción:** Muestra el historial de commits en el repositorio, con detalles como el autor, fecha y 
mensaje del commit.
- **Uso:**
  ```bash
  git log
  ```

### `git log --oneline`
- **Descripción:** Muestra el historial de commits en un formato más compacto, con un resumen de una sola linea
por commit.
- **Uso:**
  ```bash
  git log --oneline
  ```

## Comparación de cambios
### `git diff <archivo>`
- **Descipción:** Muestra las diferencias entre el archivo actual y la última versión confirmada en el repositorio.
- **Uso:**
  ```bash
  git diff <archivo>
  ```
  - **Ejemplo:**
    ```bash
    git diff archivo.txt
    ```


## Control de versiones
### `git checkout <hash>`
- **Descripción:** Cambia a una versión especificada del proyecto utilizando el hash del commit.
- **Uso:**
  ```bash
  git checkout <hash>
  ```
  - **Ejemplo:**
    ```bash
    git checkout a1b2c3d
    ```
  
## Manejo de ramas
### `git checkout -b <nombre-rama>`
- **Descirpción:** Crea una nueva rama y cambia a ella.
- **Uso:**
  ```bash
  git checkout -b <nombre-rama>
  ```
  - **Ejemplo:**
    ```bash
    git checkout -b develop
    ```

### `git branch <nombre-rama>`
- **Descirpción:** Crea una nueva rama sin cambiar a ella.
- **Uso:**
  ```bash
  git branch <nombre-rama>
  ```
  - **Ejemplo:**
    ```bash
    git branch develop
    ```

### `git branch -d <nombre-rama>`
- **Descirpción:** Elimina una rama local de forma segura (si ya se ha fusionado).
- **Uso:**
  ```bash
  git branch -d <nombre-rama>
  ```
  - **Ejemplo:**
    ```bash
    git branch -d vieja-rama
    ```

### `git branch -D <nombre-rama>`
- **Descirpción:** Fuerza la eliminación de una rama local, incluso si no ha sido fusionada.
- **Uso:**
  ```bash
  git branch -D <nombre-rama>
  ```
  - **Ejemplo:**
    ```bash
    git branch -D vieja-rama
    ```

### `git checkout <nombre-rama>`
- **Descirpción:** Cambia de la rama actual a la rama especificada.
- **Uso:**
  ```bash
  git checkout <nombre-rama>
  ```
  - **Ejemplo:**
    ```bash
    git checkout main
    ```

### `git branch`
- **Descirpción:** Muestra la lista de ramas existentes en el repositorio, con un asterisco indicando la rama activa.
- **Uso:**
  ```bash
  git branch
  ```