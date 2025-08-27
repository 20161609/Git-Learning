# 🚀 Git Learning Step 3: Work with Branches & Collaboration

## ✅ Goal
- Understand **branches** and why they're useful  
- Learn to create, switch, merge, and delete branches  
- Practice a **basic collaboration workflow** with GitHub

---

## 🌿 What is a Branch?

A **branch** is an independent line of development inside your Git repository.

> 💡 Think of branches as **parallel timelines**:
> - Work on a new feature without touching the main code
> - Experiment safely without breaking production
> - Merge changes when they're ready

---

## 🛠️ Basic Branch Commands

| Command | Description |
| --- | --- |
| `git branch` | Show all local branches |
| `git branch <name>` | Create a new branch |
| `git switch <name>` | Switch to another branch *(Git 2.23+)* |
| `git checkout <name>` | Switch branch *(older Git syntax)* |
| `git merge <name>` | Merge another branch into current branch |
| `git branch -d <name>` | Delete a local branch |
| `git push origin <name>` | Push a local branch to GitHub |
| `git pull origin <name>` | Pull remote changes into current branch |

---

## 📌 Example Workflow

```bash
# 1. Check current branch
git branch

# 2. Create a new branch
git branch feature/login

# 3. Switch to the new branch
git switch feature/login
# (Or older syntax)
git checkout feature/login

# 4. Make changes and commit
git add .
git commit -m "feat: add login UI"

# 5. Push the branch to GitHub
git push origin feature/login

# 6. Merge branch into main
git switch main
git merge feature/login

# 7. Delete local branch
git branch -d feature/login
```

---

## 🔄 Collaboration Workflow (Basic)

When working with others (or even solo for safety), follow this process:

### 1) **Update Your Local Main Branch**

```bash
git switch main
git pull origin main
```

### 2) **Create a Feature Branch**

```bash
git branch feature/calendar
git switch feature/calendar
```

### 3) **Make Changes → Commit → Push**

```bash
git add .
git commit -m "feat: add monthly calendar view"
git push origin feature/calendar
```

### 4) **Create a Pull Request (PR) on GitHub**
- Go to your repository on GitHub
- Click **Compare & pull request**
- Review changes → Merge PR

### 5) **Delete the Branch After Merging**
```bash
git branch -d feature/calendar
git push origin --delete feature/calendar
```

---

## ⚠️ Handling Merge Conflicts

Sometimes Git can’t auto-merge changes. When that happens:

1. Open the conflicted file — Git will mark conflict areas like this:
    ```diff
    <<<<<<< HEAD
    Your local changes
    =======
    Incoming changes from branch
    >>>>>>> feature/login
    ```

2. Edit the file manually to **keep the correct version**.

3. Mark conflict as resolved:
    ```bash
    git add <file>
    git commit
    ```

4. Push again:
    ```bash
    git push origin main
    ```

---

## 📖 Command Recap

| Situation | Command |
| --- | --- |
| Create branch | `git branch <name>` |
| Switch branch | `git switch <name>` |
| Push branch | `git push origin <name>` |
| Merge branch | `git merge <name>` |
| Delete branch | `git branch -d <name>` |
| Delete remote branch | `git push origin --delete <name>` |

---

## ✅ Before Moving to Step 4

By now, you should be able to:

- Understand what branches are and why they’re useful
- Create, switch, merge, and delete branches
- Push feature branches to GitHub
- Handle basic merge conflicts
- Follow a safe collaboration workflow

---

## 📚 Resources

- [Git Docs – Branching](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell)
- [GitHub Flow](https://docs.github.com/en/get-started/quickstart/github-flow)
- [Atlassian Git Branching Guide](https://www.atlassian.com/git/tutorials/using-branches)

---

## 🔗 Next Step

Go to **Step 4 – Undo Mistakes & Explore Advanced Git** to learn how to:
- Undo commits safely  
- Use `git stash` to save temporary changes  
- Rebase vs merge explained
