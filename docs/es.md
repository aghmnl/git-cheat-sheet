# Git Cheat Sheet (Español)

[Volver al Índice](index.md) | [View in English](en.md)

## Comandos Básicos

- `git init`: Inicializa un nuevo repositorio.
- `git init [nombre-proyecto]`: Inicializa un nuevo repositorio en un directorio específico.
- `git clone [url]`: Clona un repositorio desde una URL remota.
- `git status`: Muestra el estado del directorio de trabajo.

## Visualización de Cambios

- `git diff`: Muestra los cambios en el directorio de trabajo.
- `git diff --staged`: Muestra los cambios preparados para el commit.
- `git diff [primera-rama]...[segunda-rama]`: Compara diferencias entre dos ramas.
- `git log`: Muestra el historial de commits.
- `git log --follow [archivo]`: Muestra el historial de commits para un archivo, incluyendo renombramientos.
- `git show [commit]`: Muestra detalles de un commit específico.

## Ramas y Fusiones

- `git branch`: Lista las ramas locales.
- `git branch [nombre-rama]`: Crea una nueva rama.
- `git checkout -b [nombre-rama]`: Crea y cambia a una nueva rama.
- `git checkout [nombre-rama]`: Cambia a una rama existente.
- `git checkout [hash]`: Cambia a un commit específico por su hash.
- `git merge [nombre-rama]`: Fusiona una rama en la rama actual.

## Repositorios Remotos

- `git remote set-url origin [url]`: Cambia la URL del repositorio remoto.
- `git fetch`: Obtiene actualizaciones del repositorio remoto.
- `git fetch --prune`: Obtiene actualizaciones y elimina ramas remotas eliminadas.
- `git pull`: Descarga y fusiona cambios del repositorio remoto.
- `git pull [nombre-remoto] [nombre-rama]`: Descarga y fusiona cambios de la ram específica del repositorio remoto (normalmente llamado origin).
- `git push`: Sube cambios al repositorio remoto.
- `git push [nombre-remoto] [nombre-rama]`: Sube cambios a la rama específica del repositorio remoto (normalmente llamado origin).
- `git push [nombre-remoto] --delete [nombre-rama]`: Elimina una rama del respositorio remoto (normalmente llamado origin).

## Stashing

- `git stash`: Guarda cambios no confirmados.
- `git stash list`: Lista todos los stashes.
- `git stash apply`: Aplica el último stash sin eliminarlo.
- `git stash pop`: Aplica y elimina el último stash.
- `git stash drop`: Elimina el último stash.
- `git stash branch [nombre-rama] stash@{<índice>}`: Crea una rama desde un stash.

## Configuración

- `git config --global user.name "[nombre]"`: Configura el nombre de usuario global.
- `git config --global user.email "[correo]"`: Configura el correo electrónico global.
- `git config --list`: Lista todas las configuraciones.

## Deshacer Cambios

- `git reset [commit]`: Restaura el directorio de trabajo a un commit específico.
- `git reset --hard HEAD`: Restaura el directorio de trabajo al último commit.
- `git checkout HEAD~1`: Cambia al commit anterior.
- `git rm --cached [archivo]`: Elimina un archivo del área de preparación.
- `git rm -r --cached .`: Elimina todos los archivos del área de preparación.

## Gestión de Archivos

- `git add [archivo]`: Añade un archivo específico al área de preparación.
- `git mv [archivo-original] [archivo-renombrado]`: Renombra o mueve un archivo.

## Glosario

- **Branch**: Una línea separada de desarrollo en un repositorio.
- **Commit**: Una instantánea de los cambios en el repositorio.
- **Fetch**: Descarga actualizaciones de un repositorio remoto sin fusionarlas.
- **Merge**: Combina cambios de una rama en otra.
- **Pull**: Descarga y fusiona cambios de un repositorio remoto.
- **Push**: Sube cambios a un repositorio remoto.
- **Stash**: Guarda temporalmente cambios no confirmados.
