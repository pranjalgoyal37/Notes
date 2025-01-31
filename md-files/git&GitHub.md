
# Git and GitHub Notes

## Introduction

### Git

- **Definition**: Git is a distributed version control system for tracking changes in source code during software development.
- **Key Features**:
  - Tracks history of changes.
  - Supports branching and merging.
  - Distributed architecture.
  - Efficient handling of large projects.

### GitHub

- **Definition**: GitHub is a cloud-based hosting service for managing Git repositories with added functionalities for collaboration.
- **Key Features**:
  - Repository hosting.
  - Collaboration tools (issues, pull requests, etc.).
  - GitHub Actions for CI/CD.
  - Version control with Git integration.

!["Git vs GitHub"]("./git_v_github.png")

## Git Basics

### Installation

- Install Git from [git-scm.com](https://git-scm.com).
- Verify installation:
  ```bash
  git --version
  ```

###  Git Configuration
  ```bash
  # Set global configuration for user name and email
    git config --global user.name "Your Name"
    git config --global user.email "youremail@example.com"

  # Use Visual Studio Code as default editor
    git config --global core.editor "code --wait"  

# View configuration:
  git config --list
  ```
### state change commands
```bash
git add <file>               # Add file to staging area:
git add .                       # Add all changes to staging area:
git reset  <file>           # Unstage file:
git reset --hard            # Discard all changes:
git status -s                 # Short status summary:
git diff                         # Show diff b/w working tree and staging area:
git diff --staged           # Show diff b/w staging area and committed changes:
```
### Git Commits
```bash
git commit -m "Commit message"    # Commit changes with message:
git commit -am "meesage"               # Commit changes with all tracked(modified) files:
git commit --amend               # Modify last commit message:  

  git reset --soft HEAD~1     # Reset to previous commit:
  git reset --hard HEAD~1       # Reset to previous commit and discard changes:


git log                                   # Show commit history in one line:
git log --oneline               # Show commit history in one line:
git log --graph                  # Show commit history with graph:
  ```
### Git Branch & Merge
```bash
1. git branch <branch-name>         # Create a new branch:
2. git checkout <branch-name>       # Switch to a branch:
3. git checkout -b <branch-name> # Create a new branch and switch to it:
4. git rename <old-branch> <new-branch> # Rename a branch:
5. git branch -d <branch-name>       # Delete a branch:
6. git merge <branch-name>         # Merge branch into current branch:

#Note:  
#1)- make sure you are on main branch before merging. 
#2)- if same file is modified in both branches, git will show conflict.

# resolve conflicts:
  # manually resolve conflicts (open file with conflict, resolve conflicts, save)
  # add resolved file: git add <file>
  # commit changes: git commit -m "resolved conflicts"

```
### git update local to  remote repository
```bash
  1. git remote add origin <repository-url>      # Add remote repository
  2. git push origin main               # Push all changes to remote main branch
  3. git push origin <branch-name>   # Push changes to a specific branch
  
  4. git fetch origin <branch-name>     # Fetch changes from remote branch
  5. git merge origin/<branch-name>   # Merge changes from remote branch into current branch
  
  6. git pull origin <branch-name>     # Fetch changes from remote branch, merge into current branch, and push to origin
  
  7. git branch -d <branch-name>       # Delete a local branch
  8. git push origin --delete <branch-name> # Delete a remote branch
```

- **Initialize a repository**: It initialize an empty git repo in current working dir of local machine.
  ```bash
  git init
  ```
- **Clone a repository**:
  ```bash
  git clone <repository-url>
  ```
- **Check repository status**:  ```bash
  git status
  ```
- **Stage changes**:
  ```bash
  git add <file>
  git add .
  ```
- **Commit changes**:
  ```bash
  git commit -m "Commit message"
  ```
- **View commit history**:
  ```bash
  git log
  ```

## Git Branching

- **Create a new branch**:
  ```bash
  git branch <branch-name>
  ```
- **Switch to a branch**:
  ```bash
  git checkout <branch-name>
  ```
- **Create and switch to a branch**:
  ```bash
  git checkout -b <branch-name>
  ```
- **Merge branches**:
  ```bash
  git merge <branch-name>
  ```
- **Delete a branch**:
  ```bash
  git branch -d <branch-name>
  ```

## Working with Remote Repositories

### Common Commands

- **Add a remote repository**:
  ```bash
  git remote add origin <repository-url>
  ```
- **View remotes**:
  ```bash
  git remote -v
  ```
- **Push changes**:
  ```bash
  git push origin <branch-name>
  ```
- **Pull changes**:
  ```bash
  git pull origin <branch-name>
  ```
- **Fetch changes**:
  ```bash
  git fetch
  ```

## GitHub Basics

### Repository Setup

1. Sign up on [GitHub](https://github.com).
2. Create a new repository.
3. Clone the repository locally or connect it to an existing Git repository.

### Collaboration

- **Fork a repository**: Create your copy of another repository.
- **Create a pull request**: Propose changes to a repository.
- **Resolve merge conflicts**: Fix conflicts manually and commit.

## Advanced Git Commands

- **Stash changes**:
  ```bash
  git stash
  ```
- **Apply stashed changes**:
  ```bash
  git stash apply
  ```
- **Revert a commit**:
  ```bash
  git revert <commit-hash>
  ```
- **Reset to a previous commit**:
  ```bash
  git reset --hard <commit-hash>
  ```

## Best Practices

1. Write clear and concise commit messages.
2. Use branches for feature development.
3. Regularly pull changes from the remote repository.
4. Review changes before committing.
5. Avoid committing sensitive information.

---






