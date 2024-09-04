## `git checkout -b <nombre-rama>`
- **Descripción:** Crea una nueva rama y cambia a ella en un solo paso.
- **Ejemplo de uso:**
  ```bash
  git checkout -b develop
  ```

## `git branch <nombre-rama>`
- **Descripción:** Crea una nueva rama sin cambiar a ella.
- **Ejemplo de uso:**
  ```bash
  git branch develop
  ```

## `git merge <nombre-rama>`
- **Descripción:** Fusiona la rama especificada en la rama actual. Git intentará integrar los cambios de la otra rama en tu rama activa.
- **Ejemplo de uso:**
  ```bash
  git merge develop
  ```

## `git branch -d <nombre-rama>`
- **Descripción:** Elimina una rama local de forma segura (si ya se ha fusionado).
- **Condición:** Debes estar en una rama diferente a la que deseas eliminar. La rama no puede estar activa y debe haberse fusionado previamente.
- **Ejemplo de uso:**
  ```bash
  git branch -d vieja-rama
  ```

## `git branch -D <nombre-rama>`
- **Descripción:** Fuerza la eliminación de una rama local, incluso si no ha sido fusionada.
- **Condición:** Debes estar en una rama diferente a la que deseas eliminar. Este comando debe usarse con precaución, ya que puede resultar en la pérdida de trabajo no fusionado.
- **Ejemplo de uso:**
  ```bash
  git branch -D vieja-rama
  ```

## `git checkout <nombre-rama>`
- **Descripción:** Cambia de la rama actual a la rama especificada.
- **Condición:** La rama especificada debe existir localmente. Si tienes cambios sin confirmar, debes confirmarlos o guardarlos antes de cambiar de rama.
- **Ejemplo de uso:**
  ```bash
  git checkout main
  ```

## `git branch`
- **Descripción:** Muestra la lista de ramas existentes en el repositorio, con un asterisco indicando la rama activa.
- **Ejemplo de uso:**
  ```bash
  git branch
  ```