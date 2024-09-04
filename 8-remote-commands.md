## `git push -u origin <nombre-rama>`
- **Descripción:** Sube una rama local al repositorio remoto y establece un enlace entre la rama local y la remota. Después de hacer esto, los futuros comandos git push y git pull usarán automáticamente esa rama sin necesidad de especificarla.
- **Condición:** La rama especificada debe existir localmente. Este comando se usa comúnmente la primera vez que se sube una nueva rama al repositorio remoto.
- **Ejemplo de uso:**
  ```bash
  git push -u origin main
  ```

## `git fetch`
- **Descripción:** Descarga cambios del repositorio remoto a tu repositorio local, pero *no los fusiona* en tu trabajo actual. Esto te permite revisar los cambios antes de decidir si los incorporas.
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
- **Descripción:** Envía tus cambios confirmados (commits) de tu repositorio local al repositorio remoto. Este comando es útil para compartir tu trabajo con otros.
- **Ejemplo de uso:**
  ```bash
  git push origin main
  ```

## `git fetch origin <nombre-rama>`
- **Descripción:** Descarga los cambios de una rama específica en el repositorio remoto sin fusionarlos con la rama actual en tu repositorio local. Esto es útil para revisar los cambios antes de hacer una fusión.
- **Ejemplo de uso:**
  ```bash
  git fetch origin develop
  ```

## `git pull origin <nombre-rama>`
- **Descripción:** Descarga y fusiona automáticamente los cambios de una rama específica del repositorio remoto en la rama actual. Este comando es equivalente a ejecutar git `fetch origin <nombre-rama>` seguido de `git merge <nombre-rama>`.
- **Condición:**  Debes estar en la rama local en la que deseas fusionar los cambios.
- **Ejemplo de uso:**
  ```bash
  git pull origin develop
  ```

## `git push origin <nombre-rama>`
- **Descripción:** Sube una rama local al repositorio remoto. Esto permite que la rama esté disponible en el repositorio remoto, como en GitHub.
- **Condición:** La rama especificada debe existir localmente. Una vez subida, la rama estará disponible en el repositorio remoto.
- **Ejemplo de uso:**
  ```bash
  git push origin develop
  ```

## `git push origin --delete <nombre-rama>`
- **Descripción:** Elimina una rama remota del repositorio, removiéndola de GitHub.
- **Condición:** Asegúrate de que la rama ya no sea necesaria en el repositorio remoto, ya que esta operación no se puede deshacer.
- **Ejemplo de uso:**
  ```bash
  git push origin --delete develop
  ```