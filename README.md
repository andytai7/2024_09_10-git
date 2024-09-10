# 2024_09_10-git

### Setting Up a New Repository
- **`git init`**: Initializes a new Git repository in the current directory.
- **`git remote add origin <remote_url>`**: Adds a remote repository called `origin` with the specified URL.
- **`git branch -M main`**: Renames the current branch to `main`.
- **`git push -u origin main`**: Pushes the `main` branch to the remote repository and sets it as the default upstream branch.

### Working with Changes
- **`git restore <file>`**: Restores the specified file to the last committed state in the working directory.
- **`git restore --staged <file>`**: Unstages a file, moving it back from the staging area to the working directory.

### Viewing Differences
- **`git diff <file>`**: Shows the differences between the working directory and the staging area for the specified file.
- **`git diff --staged <file>`**: Displays changes that have been staged but not yet committed.

### Viewing the Commit History
- **`git log --oneline`**: Displays the commit history in a simplified, one-line-per-commit format.
    - Press `q` to exit the log if it overflows the screen.

### Undoing Changes
- **`git restore --source <hash> <file>`**: Restores a specific version of a file from a previous commit using its commit hash.

### Managing Merges
- **`git config pull.rebase false`**: Ensures that `git pull` uses merge instead of rebase.
- **`git pull origin main`**: Fetches and merges changes from the `main` branch of the remote repository.
- **`git merge --abort`**: Aborts an ongoing merge process if conflicts or issues arise.

### Stashing Changes
- **`git stash`**: Saves the current changes in a temporary storage, allowing you to work on other tasks without committing them.
- **`git stash pop`**: Applies the most recent stash and removes it from the stash list.
