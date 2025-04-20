# Git Cheat Sheet (English)

## Basic Commands

These commands are used to initialize, clone, and check the status of a repository.

- `git init`: Initialize a new repository in the current directory.
  - Example: `git init`
- `git init [project-name]`: Initialize a new repository in a specific directory.
  - Example: `git init my-project`
- `git clone [url]`: Clone a repository from a remote URL.
  - Example: `git clone https://github.com/user/repo.git`
- `git status`: Show the working directory status.
  - Example: `git status`

## Viewing Changes

Commands to view differences between commits, branches, or the working directory.

- `git diff`: Show changes in the working directory.
  - Example: `git diff`
- `git diff --staged`: Show changes staged for commit.
  - Example: `git diff --staged`
- `git diff [first-branch]...[second-branch]`: Compare differences between two branches.
  - Example: `git diff main...feature-branch`
- `git log`: Show commit history.
  - Example: `git log`
- `git log --follow [file]`: Show commit history for a file, including renames.
  - Example: `git log --follow README.md`
- `git show [commit]`: Show details of a specific commit.
  - Example: `git show abc123`

## Branching and Merging

Commands to manage branches and merge changes.

- `git branch`: List local branches.
  - Example: `git branch`
- `git branch [branch-name]`: Create a new branch.
  - Example: `git branch feature`
- `git checkout -b [branch-name]`: Create and switch to a new branch.
  - Example: `git checkout -b feature`
- `git checkout [branch-name]`: Switch to an existing branch.
  - Example: `git checkout main`
- `git checkout [hash]`: Check out a specific commit by its hash.
  - Example: `git checkout abc123`
- `git merge [branch-name]`: Merge a branch into the current branch.
  - Example: `git merge feature`

## Remote Repositories

Commands to interact with remote repositories.

- `git remote set-url origin [url]`: Change the remote repository URL.
  - Example: `git remote set-url origin https://github.com/user/repo.git`
- `git fetch`: Fetch updates from the remote repository.
  - Example: `git fetch`
- `git fetch --prune`: Fetch updates and remove deleted remote branches.
  - Example: `git fetch --prune`
- `git pull`: Fetch and merge changes from the remote repository.
  - Example: `git pull`
- `git push`: Push changes to the remote repository.
  - Example: `git push`
- `git push origin --delete [branch-name]`: Delete a remote branch.
  - Example: `git push origin --delete feature`

## Stashing

Commands to save and manage uncommitted changes.

- `git stash`: Save uncommitted changes.
  - Example: `git stash`
- `git stash list`: List all stashes.
  - Example: `git stash list`
- `git stash apply`: Apply the latest stash without removing it.
  - Example: `git stash apply`
- `git stash pop`: Apply and remove the latest stash.
  - Example: `git stash pop`
- `git stash drop`: Delete the latest stash.
  - Example: `git stash drop`
- `git stash branch [branch-name] stash@{<index>}`: Create a branch from a stash.
  - Example: `git stash branch feature stash@{0}`

## Configuration

Commands to configure Git settings.

- `git config --global user.name "[name]"`: Set the global username.
  - Example: `git config --global user.name "John Doe"`
- `git config --global user.email "[email address]"`: Set the global email address.
  - Example: `git config --global user.email "john.doe@example.com"`
- `git config --list`: List all configuration settings.
  - Example: `git config --list`

## Undoing Changes

Commands to undo changes in the working directory or repository.

- `git reset [commit]`: Reset the working directory to a specific commit.
  - Example: `git reset abc123`
- `git reset --hard HEAD`: Reset the working directory to the last commit.
  - Example: `git reset --hard HEAD`
- `git checkout HEAD~1`: Check out the previous commit.
  - Example: `git checkout HEAD~1`
- `git rm --cached [file]`: Remove a file from the staging area.
  - Example: `git rm --cached file.txt`
- `git rm -r --cached .`: Remove all files from the staging area.
  - Example: `git rm -r --cached .`

## File Management

Commands to manage files in the repository.

- `git add [file]`: Stage a specific file for commit.
  - Example: `git add README.md`
- `git mv [file-original] [file-renamed]`: Rename or move a file.
  - Example: `git mv old-name.txt new-name.txt`
