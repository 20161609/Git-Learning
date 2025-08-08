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
