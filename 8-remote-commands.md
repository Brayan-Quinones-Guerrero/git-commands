## `git fetch`
- **Descripción:** Descarga los cambios de un repositorio remoto, actualizando las referencias de las ramas remotas en tu repositorio local, pero sin fusionarlos con la rama de trabajo actual. Es útil para revisar los cambios antes de hacer una fusión.
- **Ejemplo de uso:**
  ```bash
  git fetch origin
  ```

## `git pull`
- **Descripción:** Descarga y fusiona automáticamente los cambios del repositorio remoto en la rama actual. Este comando es equivalente a ejecutar `git fetch` seguido de `git merge`. Puede causar conflictos si hay cambios conflictivos entre la rama remota y tu rama local.
- **Ejemplo de uso:**
  ```bash
  git pull origin main
  ```

## `git push`
- **Descripción:** Envía los commits locales al repositorio remoto.
- **Ejemplo de uso:**
  ```bash
  git push origin main
  ```