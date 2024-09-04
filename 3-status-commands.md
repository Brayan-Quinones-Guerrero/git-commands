## `git status`
- **Descripción:** Muestra el estado del repositorio, indicando archivos modificados, agregados y no rastreados.
- **Ejemplo de uso:**
  ```bash
  git status
  ```

## `git status -s`
- **Descripción:** Muestra el estado del repositorio de manera abreviada, utilizando letras para indicar el estado de los archivos.
- **Descripción detallada de los indicadores:**
  - `??`: El archivo no está siendo rastreado por Git (untracked).
  - `M`: El archivo ha sido modificado.
  - `D`: El archivo ha sido eliminado.
  - `R`: El archivo ha sido renombrado.
  - `C`: El archivo ha sido copiado.
  - `A`: El archivo ha sido agregado al área de preparación.
  - `U`: Hay un conflicto de fusión en el archivo.
  Los indicadores de estado pueden aparecer en dos columnas:
    - **Primera columna:** Indica el estado del archivo en el área de preparación (staging area).
    - **Segunda columna:** Indica el estado del archivo en el directorio de trabajo.
  - **Por ejemplo:**
    ```bash
    M  archivo.txt   # Modificado en el área de trabajo, no preparado para commit
    AM archivo.txt   # Agregado al área de preparación y modificado después
    A  archivo.txt   # Archivo agregado al área de preparación
    D  archivo.txt   # Eliminado del área de trabajo y marcado para eliminación
    ```
- **Ejemplo de uso:**
  ```bash
  git status -s
  ```