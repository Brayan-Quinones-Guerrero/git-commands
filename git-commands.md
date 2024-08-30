# GIT Commands

## Inicialización del Repositorio
### `git init`
- **Descripción:** Inicializa un nuevo repositorio Git en el directorio actual.


## Manejo de Archivos
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
- **Descripción:** Agrega todos los archivos modificados y nuevos del directorio actual al área de preparación.
- **Ejemplo de uso:**
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

## Estado del Repositorio
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

## Confirmación de Cambios
### `git commit -m`
- **Descripción:** Confirma los cambios agregados al área de preparación en el repositorio, con un mensaje de confirmación.
- **Uso:**
  ```bash
  git commit -m "mensaje"
  ```
  - **Ejemplo:**
    ```bash
    git commit -m "Agregados nuevos archivos al proyecto"
    ```
