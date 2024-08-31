# GIT Commands


## Inicialización del repositorio
### `git init`
- **Descripción:** Inicializa un nuevo repositorio Git en el directorio actual.
- **Uso:**
  ```bash
  git init
  ```


## Manejo de archivos
### `git add`
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
- **Descripción:** Agrega todos los archivos modificados y nuevos del **directorio actual** al área de preparación.
- **Uso:**
  ```bash
  git add .
  ```

### `git rm --cached`
- **Descripción:** Elimina un archivo del área de preparación sin eliminarlo del sistema de archivos.
- **Uso:**
  ```bash
  git rm --cached <archivo>
  ```
  - **Ejemplo:**
    ```bash
    git rm --cached archivo.txt
    ```

### `git rm --cached -f`
- **Descripción:** Fuerza la eliminación de un archivo del área de preparación.
- **Uso:**
  ```bash
  git rm --cached -f <archivo>
  ```
  - **Ejemplo:**
    ```bash
    git rm --cached -f archivo.txt
    ```
  
### `git restore`
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
- **Descripción:** Añade todos los archivos **modificados** al área de preparación y los confirma con un mensaje, todo en un solo paso.
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