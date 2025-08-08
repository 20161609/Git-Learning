# 🧠 Git Learning Step 1: Understand the Basics

## ✅ Goal
- Understand what Git is and why it's used
- Use basic Git commands to start version control in a local project

---

## 🚀 What is Git?

Git is a **distributed version control system (VCS)** that helps you track code changes, work on features safely, and collaborate with others.

> 💡 Why Git?
> - Keep history of changes
> - Undo mistakes and go back to previous versions
> - Work in parallel using branches
> - Collaborate without stepping on each other's toes

---

## 🛠️ Installing Git

### 🖥️ Windows
Download and install from [git-scm.com](https://git-scm.com/download/win)  
Use **Git Bash** for terminal commands

### 🍎 macOS
If you have Homebrew:
```bash
brew install git
```

## ✨ Essential Git Commands

| Command | Description |
| --- | --- |
| `git init` | Initialize a Git repository in the current folder |
| `git status` | Check status of tracked/untracked files |
| `git add <filename>` | Stage a specific file for commit |
| `git add .` | Stage all changed files |
| `git commit -m "message"` | Save staged changes with a commit message |
| `git log` | Show commit history |

---

## 📌 Example Workflow

```bash
# 1. Create a new project folder
mkdir my-project
cd my-project

# 2. Initialize Git
git init

# 3. Create a file and check status
touch index.html
git status

# 4. Stage the file
git add index.html

# 5. Commit the file
git commit -m "Initial commit"

# 6. View commit history
git log

```

---

## 📖 Command Breakdown

### `git init`

Initializes a new Git repository in the current folder. Creates a hidden `.git` directory to store version history.

### `git add .`

Stages all changes (new, modified, deleted files) for the next commit.

### `git commit -m "message"`

Saves the staged changes as a commit with a descriptive message.

### `git status`

Shows the current state of your working directory and staging area.

### `git log`

Displays commit history with IDs, authors, and dates.

---

## ✅ Before Moving to Step 2

You should be able to:

- Initialize a repository
- Stage and commit files
- View commit history

---

## 🔗 Next Step

Go to **Step 2 – Connect to GitHub & Use Remote Repositories** to learn how to push your local project to GitHub.

---

## 📚 Resources

- [Pro Git Book (Free)](https://git-scm.com/book/en/v2)
- [GitHub Docs](https://docs.github.com/en)
- [Git Cheat Sheet PDF](https://education.github.com/git-cheat-sheet-education.pdf)