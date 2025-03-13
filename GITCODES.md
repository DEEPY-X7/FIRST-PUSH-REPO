# Comprehensive Git Commands Guide

## 1. Initializing and Configuring Git
```sh
git init  # Initialize a new Git repository
git config --global user.name "DEEPY.X7"  # Set global username
git config --global user.email "your email"  # Set global email address
git config --list  # View all global Git configurations
```

## 2. Staging and Committing Changes
```sh
git add .  # Add all files to the staging area
git add -A  # Add all changes, including deletions
git add filename  # Add a specific file to the staging area
git status  # Check the current state of the repository
git commit -m "Commit message"  # Commit staged changes with a message
git commit -a -m "Commit message"  # Commit all changes without using 'git add'
git commit --amend -m "Updated commit message"  # Modify the last commit message
```

## 3. Managing Files
```sh
touch filename  # Create a new file (e.g., touch index.html)
ls  # List all files in the current directory
git rm filename  # Delete a file and stage the removal
git rm --cached filename  # Remove a file from tracking but keep it locally
git mv old_filename new_filename  # Rename or move a file
```

## 4. Checking and Reverting Changes
```sh
git log  # View commit history
git log --oneline  # Display commit history in a compact format
git log -p -n<number>  # Show detailed changes in last 'n' commits
git diff  # Compare working directory with the last commit
git diff --staged  # Show changes between staging area and last commit
git checkout filename  # Restore a file to its last committed state
git checkout -f  # Revert all files to the last committed state
git reset HEAD filename  # Unstage a file but keep changes in working directory
git reset --soft HEAD~1  # Undo last commit but keep changes staged
git reset --hard HEAD~1  # Undo last commit and discard changes permanently
git revert <commit_hash>  # Create a new commit that undoes a specific commit
```

## 5. Branching and Merging
```sh
git branch  # List all branches
git branch branch_name  # Create a new branch
git checkout branch_name  # Switch to a specific branch
git checkout -b branch_name  # Create and switch to a new branch
git merge branch_name  # Merge a branch into the current branch
git branch -d branch_name  # Delete a local branch
git push origin --delete branch_name  # Delete a remote branch
```

## 6. Working with Remote Repositories
```sh
git remote add origin <repository_url>  # Link local repo to a remote repository
git remote -v  # View linked remote repositories
git fetch  # Download changes from remote without applying them
git pull origin main  # Fetch and merge changes from remote main branch
git push origin main  # Push local commits to the remote main branch
git push -u origin branch_name  # Push a new branch to the remote repository
```

## 7. Stashing and Cleaning
```sh
git stash  # Save uncommitted changes temporarily
git stash list  # View stashed changes
git stash pop  # Apply stashed changes and remove from stash list
git stash apply  # Apply stashed changes without removing from stash list
git stash drop  # Delete a specific stash
git clean -n  # Show files that will be removed
git clean -f  # Remove untracked files permanently
```

## 8. Miscellaneous Commands
```sh
git show <commit_hash>  # View details of a specific commit
git tag tag_name  # Create a tag for a commit
git tag -a tag_name -m "Tag message"  # Create an annotated tag
git push origin --tags  # Push all local tags to the remote repository
clear  # Clear terminal screen
```

### Notes:
- If any command is unclear, refer to online documentation or search for more details.
- Git commands are powerful; use them carefully to avoid losing important work.
- Version control helps track changes and manage collaborative development efficiently.
