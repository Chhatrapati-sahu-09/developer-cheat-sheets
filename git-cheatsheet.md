<p align="center">
<img src="https://cdn.simpleicons.org/git/F05032" height="70" alt="Git"/>
</p>

# Git Cheat Sheet

Git is a distributed version control system that allows developers to track changes in source code, collaborate with others, and maintain different versions of a project. It is widely used in software development to manage code efficiently.

This cheat sheet provides a quick reference for commonly used Git commands.

---

## Repository Setup

<img src="https://cdn.simpleicons.org/github" height="22"/> These commands are used to create or download a repository.

| Command                      | Description                                                                   |
| ---------------------------- | ----------------------------------------------------------------------------- |
| `git init`                   | Initializes a new Git repository in the current directory.                    |
| `git clone <repository_url>` | Creates a copy of an existing repository from a remote source such as GitHub. |

Example:

```bash
git clone https://github.com/user/project.git
```

---

## Checking Repository Status

<img src="https://cdn.simpleicons.org/git/F05032" height="22"/> These commands help you inspect the current state of your repository.

| Command      | Description                                                            |
| ------------ | ---------------------------------------------------------------------- |
| `git status` | Displays the current status of the working directory and staging area. |

Example:

```bash
git status
```

This command shows:

* modified files
* staged files
* untracked files

---

## Staging Changes

<img src="https://cdn.simpleicons.org/git/F05032" height="22"/> Before committing changes, files must be added to the staging area.

| Command          | Description                                                           |
| ---------------- | --------------------------------------------------------------------- |
| `git add <file>` | Adds a specific file to the staging area.                             |
| `git add .`      | Adds all modified files in the current directory to the staging area. |

Example:

```bash
git add index.js
```

---

## Committing Changes

<img src="https://cdn.simpleicons.org/git/F05032" height="22"/> A commit saves a snapshot of your staged changes in the repository history.

| Command                   | Description                                                   |
| ------------------------- | ------------------------------------------------------------- |
| `git commit -m "message"` | Records the staged changes with a descriptive commit message. |

Example:

```bash
git commit -m "Add login feature"
```

Good commit messages help other developers understand what changes were made.

---

## Working with Remote Repositories

<img src="https://cdn.simpleicons.org/github" height="22"/> Remote repositories allow collaboration with other developers.

| Command                    | Description                                              |
| -------------------------- | -------------------------------------------------------- |
| `git push origin <branch>` | Uploads local commits to the remote repository.          |
| `git pull origin <branch>` | Downloads the latest changes from the remote repository. |

Example:

```bash
git push origin main
```

---

## Branch Management

<img src="https://cdn.simpleicons.org/git/F05032" height="22"/> Branches allow developers to work on features or fixes without affecting the main codebase.

| Command                         | Description                                          |
| ------------------------------- | ---------------------------------------------------- |
| `git branch <branch_name>`      | Creates a new branch.                                |
| `git checkout <branch_name>`    | Switches to another branch.                          |
| `git checkout -b <branch_name>` | Creates a new branch and switches to it immediately. |
| `git merge <branch_name>`       | Merges another branch into the current branch.       |
| `git branch -d <branch_name>`   | Deletes a branch after it has been merged.           |

Example:

```bash
git checkout -b feature-login
```

---

## Useful Workflow Example

<img src="https://cdn.simpleicons.org/git/F05032" height="22"/> A typical Git workflow may look like this:

```bash
git clone repository_url
git checkout -b new-feature
git add .
git commit -m "Implement new feature"
git push origin new-feature
```

This workflow allows developers to safely work on new features before merging them into the main branch.

---

## Summary

Git helps developers manage code changes, collaborate with teams, and maintain a clear project history. Understanding these basic commands is essential for efficient version control and modern software development workflows.
