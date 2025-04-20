# Git Cheat Sheet (English)

[Back to Index](index.md) | [Ver en Español](es.md)

## Basic Commands

- `git init`: Initialize a new repository.
- `git init [project-name]`: Initialize a new repository in a specific directory.
- `git clone [url]`: Clone a repository from a remote URL.
- `git status`: Show the working directory status.

## Viewing Changes

- `git diff`: Show changes in the working directory.
- `git diff --staged`: Show changes staged for commit.
- `git diff [first-branch]...[second-branch]`: Compare differences between two branches.
- `git log`: Show commit history.
- `git log --follow [file]`: Show commit history for a file, including renames.
- `git show [commit]`: Show details of a specific commit.

## Branching and Merging

- `git branch`: List local branches.
- `git branch [branch-name]`: Create a new branch.
- `git checkout -b [branch-name]`: Create and switch to a new branch.
- `git checkout [branch-name]`: Switch to an existing branch.
- `git checkout [hash]`: Check out a specific commit by its hash.
- `git merge [branch-name]`: Merge a branch into the current branch.

## Remote Repositories

- `git remote set-url origin [url]`: Change the remote repository URL.
- `git fetch`: Fetch updates from the remote repository.
- `git fetch --prune`: Fetch updates and remove deleted remote branches.
- `git pull`: Fetch and merge changes from the remote repository.
- `git pull [remote-name] [branch-name]`: Fetch and merge changes from the specific branch of the remote repository (tipically called origin).
- `git push`: Push changes to the remote repository.
- `git push [remote-name] [branch-name]`: Push changes to the specific branch of the remote repository (tipically called origin).
- `git push [remote-name] --delete [branch-name]`: Delete a branch of the remote repository (tipically called origin).

## Stashing

- `git stash`: Save uncommitted changes.
- `git stash list`: List all stashes.
- `git stash apply`: Apply the latest stash without removing it.
- `git stash pop`: Apply and remove the latest stash.
- `git stash drop`: Delete the latest stash.
- `git stash branch [branch-name] stash@{<index>}`: Create a branch from a stash.

## Configuration

- `git config --global user.name "[name]"`: Set the global username.
- `git config --global user.email "[email address]"`: Set the global email address.
- `git config --list`: List all configuration settings.

## Undoing Changes

- `git reset [commit]`: Reset the working directory to a specific commit.
- `git reset --hard HEAD`: Reset the working directory to the last commit.
- `git checkout HEAD~1`: Check out the previous commit.
- `git rm --cached [file]`: Remove a file from the staging area.
- `git rm -r --cached .`: Remove all files from the staging area.

## File Management

- `git add [file]`: Stage a specific file for commit.
- `git mv [file-original] [file-renamed]`: Rename or move a file.

## Glossary

- **Branch**: A separate line of development in a repository.
- **Commit**: A snapshot of changes in the repository.
- **Fetch**: Download updates from a remote repository without merging them.
- **Merge**: Combine changes from one branch into another.
- **Pull**: Fetch and merge changes from a remote repository.
- **Push**: Upload changes to a remote repository.
- **Stash**: Temporarily save uncommitted changes.
