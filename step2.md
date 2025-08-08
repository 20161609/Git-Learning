# 🚀 Git Learning Step 2: Connect to GitHub & Use Remote Repositories

## ✅ Goal
- Create a GitHub repository
- Connect your local project to GitHub
- Push and pull code between local and remote

---

## 🧠 What is a Remote Repository?

A remote repository is a version of your project hosted on the internet (e.g., GitHub).
It allows:
- Backup of your local project
- Collaboration with others
- Easy sharing and deployment

---

## 🛠️ Prerequisites

- Git is already installed
- You’ve completed [Step 1](./step1.md)
- You have a GitHub account → [Sign up here](https://github.com)

---

## 🔗 Create a GitHub Repository

1. Go to [https://github.com](https://github.com)
2. Click on **New repository**
3. Name it (e.g. `my-project`)
4. Do NOT check "Initialize with README" (you already have local code)
5. Click **Create repository**

---

## 🔄 Connect Local Repository to GitHub

Assuming you're inside a Git-tracked local folder:

```bash
# Set the remote repository
git remote add origin https://github.com/your-username/my-project.git

# Push local code to GitHub (first time)
git push -u origin main
```

### 📖 Command Breakdown

### 1) `git remote add origin https://github.com/your-username/my-project.git`

- **`git`** → Runs the Git program
- **`remote`** → Manages connections to other repositories
- **`add`** → Adds a new remote connection
- **`origin`** → The default name for the remote repository
    
    *(You can name it differently, but `origin` is the standard)*
    
- **`https://github.com/your-username/my-project.git`** → The URL of your remote GitHub repository

💡 **Purpose:**

Links your local repository to a remote one so you can push/pull changes.

---

### 2) `git push -u origin main`

- **`git`** → Runs the Git program
- **`push`** → Uploads local commits to a remote repository
- **`u`** → Sets the upstream tracking branch
    
    *(Future pushes/pulls won’t need `origin main` explicitly)*
    
- **`origin`** → The name of the remote repository
- **`main`** → The branch you are pushing
    
    *(Could be `master` or any other branch name)*
    

💡 **Purpose:**

Sends your committed changes to GitHub and links the local branch to the remote branch.

💡 **Tip:**

After this first push, you can simply run:

```bash
git push
git pull

```

without typing `origin main` each time.

---

## ⬇️ Clone a GitHub Repository (optional)

If you want to copy an existing GitHub repo to your computer:

```bash
git clone https://github.com/username/repo-name.git

```

---

## 🔄 Common Remote Commands

| Command | Description |
| --- | --- |
| `git remote -v` | View current remote repositories |
| `git push origin main` | Push local commits to GitHub |
| `git pull origin main` | Fetch and merge changes from GitHub |
| `git clone URL` | Clone an entire repo from GitHub |

---

## 📌 Example Workflow

```bash
# Initialize project locally
git init
git add .
git commit -m "Initial commit"

# Connect to GitHub
git remote add origin https://github.com/yourname/git-learning.git

# Push to GitHub
git push -u origin main

```

---

## ✅ Before Moving to Step 3

Make sure you:

- Can create and push to a GitHub repository
- Understand how to pull and clone
- Know the difference between local and remote

---

## 📚 Resources

- [GitHub Docs – Adding a Remote](https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories)
- [How to Push Code to GitHub (freeCodeCamp)](https://www.freecodecamp.org/news/push-to-github/)
- [GitHub CLI (Optional)](https://cli.github.com/)