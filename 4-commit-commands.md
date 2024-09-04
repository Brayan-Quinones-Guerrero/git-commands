## `git commit -m "message"`
- **Descripción:** Confirma los cambios agregados al área de preparación en el repositorio, con un mensaje de confirmación.
- **Ejemplo de uso:**
  ```bash
  git commit -m "Primer commit"
  ```

## `git commit -am "message"`
- **Descripción:** Añade todos los archivos *modificados* (excluyendo archivos nuevos) al área de preparación y los confirma con un mensaje, todo en un solo paso. Este comando es útil para confirmar rápidamente cambios en archivos que ya están siendo rastreados por Git.
- **Condición:** Este comando no agrega archivos nuevos al área de preparación, solo los modificados.
- **Ejemplo de uso:**
  ```bash
  git commit -am "Modificaciones rápidas"
  ```