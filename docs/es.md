# Git Cheat Sheet (Español)

## Comandos Básicos

Estos comandos se usan para inicializar, clonar y verificar el estado de un repositorio.

- `git init`: Inicializa un nuevo repositorio en el directorio actual.
  - Ejemplo: `git init`
- `git init [nombre-proyecto]`: Inicializa un nuevo repositorio en un directorio específico.
  - Ejemplo: `git init mi-proyecto`
- `git clone [url]`: Clona un repositorio desde una URL remota.
  - Ejemplo: `git clone https://github.com/usuario/repositorio.git`
- `git status`: Muestra el estado del directorio de trabajo.
  - Ejemplo: `git status`

## Visualización de Cambios

Comandos para ver diferencias entre commits, ramas o el directorio de trabajo.

- `git diff`: Muestra los cambios en el directorio de trabajo.
  - Ejemplo: `git diff`
- `git diff --staged`: Muestra los cambios preparados para el commit.
  - Ejemplo: `git diff --staged`
- `git diff [primera-rama]...[segunda-rama]`: Compara diferencias entre dos ramas.
  - Ejemplo: `git diff main...rama-feature`
- `git log`: Muestra el historial de commits.
  - Ejemplo: `git log`
- `git log --follow [archivo]`: Muestra el historial de commits para un archivo, incluyendo renombramientos.
  - Ejemplo: `git log --follow README.md`
- `git show [commit]`: Muestra detalles de un commit específico.
  - Ejemplo: `git show abc123`

## Ramas y Fusiones

Comandos para gestionar ramas y fusionar cambios.

- `git branch`: Lista las ramas locales.
  - Ejemplo: `git branch`
- `git branch [nombre-rama]`: Crea una nueva rama.
  - Ejemplo: `git branch feature`
- `git checkout -b [nombre-rama]`: Crea y cambia a una nueva rama.
  - Ejemplo: `git checkout -b feature`
- `git checkout [nombre-rama]`: Cambia a una rama existente.
  - Ejemplo: `git checkout main`
- `git checkout [hash]`: Cambia a un commit específico por su hash.
  - Ejemplo: `git checkout abc123`
- `git merge [nombre-rama]`: Fusiona una rama en la rama actual.
  - Ejemplo: `git merge feature`

## Repositorios Remotos

Comandos para interactuar con repositorios remotos.

- `git remote set-url origin [url]`: Cambia la URL del repositorio remoto.
  - Ejemplo: `git remote set-url origin https://github.com/usuario/repositorio.git`
- `git fetch`: Obtiene actualizaciones del repositorio remoto.
  - Ejemplo: `git fetch`
- `git fetch --prune`: Obtiene actualizaciones y elimina ramas remotas eliminadas.
  - Ejemplo: `git fetch --prune`
- `git pull`: Descarga y fusiona cambios del repositorio remoto.
  - Ejemplo: `git pull`
- `git push`: Sube cambios al repositorio remoto.
  - Ejemplo: `git push`
- `git push origin --delete [nombre-rama]`: Elimina una rama remota.
  - Ejemplo: `git push origin --delete feature`

## Stashing

Comandos para guardar y gestionar cambios no confirmados.

- `git stash`: Guarda cambios no confirmados.
  - Ejemplo: `git stash`
- `git stash list`: Lista todos los stashes.
  - Ejemplo: `git stash list`
- `git stash apply`: Aplica el último stash sin eliminarlo.
  - Ejemplo: `git stash apply`
- `git stash pop`: Aplica y elimina el último stash.
  - Ejemplo: `git stash pop`
- `git stash drop`: Elimina el último stash.
  - Ejemplo: `git stash drop`
- `git stash branch [nombre-rama] stash@{<índice>}`: Crea una rama desde un stash.
  - Ejemplo: `git stash branch feature stash@{0}`

## Configuración

Comandos para configurar ajustes de Git.

- `git config --global user.name "[nombre]"`: Configura el nombre de usuario global.
  - Ejemplo: `git config --global user.name "Juan Pérez"`
- `git config --global user.email "[correo]"`: Configura el correo electrónico global.
  - Ejemplo: `git config --global user.email "juan.perez@ejemplo.com"`
- `git config --list`: Lista todas las configuraciones.
  - Ejemplo: `git config --list`

## Deshacer Cambios

Comandos para deshacer cambios en el directorio de trabajo o repositorio.

- `git reset [commit]`: Restaura el directorio de trabajo a un commit específico.
  - Ejemplo: `git reset abc123`
- `git reset --hard HEAD`: Restaura el directorio de trabajo al último commit.
  - Ejemplo: `git reset --hard HEAD`
- `git checkout HEAD~1`: Cambia al commit anterior.
  - Ejemplo: `git checkout HEAD~1`
- `git rm --cached [archivo]`: Elimina un archivo del área de preparación.
  - Ejemplo: `git rm --cached archivo.txt`
- `git rm -r --cached .`: Elimina todos los archivos del área de preparación.
  - Ejemplo: `git rm -r --cached .`

## Gestión de Archivos

Comandos para gestionar archivos en el repositorio.

- `git add [archivo]`: Añade un archivo específico al área de preparación.
  - Ejemplo: `git add README.md`
- `git mv [archivo-original] [archivo-renombrado]`: Renombra o mueve un archivo.
  - Ejemplo: `git mv nombre-viejo.txt nombre-nuevo.txt`
