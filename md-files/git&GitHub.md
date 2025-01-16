
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

### Configuration

- Set user name and email:
  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "youremail@example.com"
  ```
- View configuration:
  ```bash
  git config --list
  ```

### Common Commands

- **Initialize a repository**: It initialize an empty git repo in current working dir of local machine.
  ```bash
  git init
  ```
- **Clone a repository**:
  ```bash
  git clone <repository-url>
  ```
- **Check repository status**:
  ```bash
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
