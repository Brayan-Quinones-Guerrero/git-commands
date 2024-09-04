## Conflictos de fusión
- **Descripción:** Los conflictos de fusión ocurren cuando Git no puede fusionar automáticamente los cambios debido a modificaciones conflictivas en los archivos. En estos casos, Git marca los conflictos en los archivos afectados.
- **Proceso de resolución:**
  1. Revisa los archivos en conflicto marcados por Git (puedes usar `git status` para ver la lista de archivos en conflicto).
  2. Edita manualmente los archivos para resolver los conflictos. Git marcará las secciones conflictivas con los siguientes marcadores:
    - `<<<<<<< HEAD`: Indica el inicio de la sección con los cambios en la rama actual.
    - `=======`: Separa los cambios entre las dos ramas en conflicto.
    - `>>>>>>> nombre-rama`: Indica el final de la sección con los cambios en la rama que estás intentando fusionar.
  3. Selecciona los cambios correctos o combina manualmente ambos conjuntos de cambios, eliminando los marcadores de conflicto.
  4. Una vez resueltos los conflictos, agrega los archivos resueltos al área de preparación con `git add`.
  5. Completa la fusión confirmando los cambios con `git commit`.
- **Ejemplo práctico:**
  Supongamos que tienes un conflicto en `archivo.txt`:
  ```bash
  <<<<<<< HEAD
  Esta es la línea desde la rama principal.
  =======
  Esta es la línea desde la rama en conflicto.
  >>>>>>> nombre-rama
  ```
  Para resolverlo, decides que quieres combinar ambos cambios:
  ```bash
  Esta es la línea desde la rama principal.
  Esta es la línea desde la rama en conflicto.
  ```
  - **Nota:** Después de resolver los conflictos y confirmar los cambios, asegúrate de revisar el resultado final para garantizar que todos los conflictos fueron resueltos correctamente y que el archivo se comporta como se espera.
- **Comandos útiles:**
  ```bash
  git status          # Verifica los archivos en conflicto
  git add archivo.txt # Marca un archivo resuelto
  git commit          # Confirma la resolución de conflictos
  ```