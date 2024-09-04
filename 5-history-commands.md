## `git log`
- **Descripción:** Muestra el historial de commits en el repositorio, con detalles como el autor, fecha y 
mensaje del commit.
- **Ejemplo de uso:**
  ```bash
  git log
  ```

## `git log --oneline`
- **Descripción:** Muestra el historial de commits en un formato más compacto, con un resumen de una sola linea
por commit.
- **Ejemplo de uso:**
  ```bash
  git log --oneline
  ```

## `git diff <archivo>`
- **Descripción:** Muestra las diferencias entre el archivo actual y la última versión confirmada en el repositorio. Este comando es útil para revisar los cambios antes de confirmarlos.
- **Ejemplo de uso:**
  ```bash
  git diff archivo.txt
  ```

## `git checkout <hash>`
- **Descripción:** Cambia a una versión especificada del proyecto utilizando el hash del commit. Esto te permite explorar el historial del proyecto en un estado anterior.
- **Ejemplo de uso:**
  ```bash
  git checkout a1b2c3d
  ```