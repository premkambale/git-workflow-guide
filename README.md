# 🚀 Git Branch Hierarchy & Workflow Guide

## 📂 Branch Hierarchy

```
Project
│
├── Frontend
│   ├── project-frontend
│   │   ├── main
│   │   ├── production
│   │   ├── UserAcceptanceTesting (UAT)
│   │   ├── dev
│   │       ├── developer1  → VS Code
│   │       ├── developer2 → VS Code
│   │       ├── developer3 → VS Code
│   │       ├── git clone -b <branch_name> <repo_url>
│
├── Backend
│
├── Devs
```

---

## 🔧 Git Workflow Commands

> **Note:** If you haven't already, create a GitLab account using your organizational email before proceeding.

### 1️⃣ Cloning a specific branch  
```sh
git clone -b <branch_name> <repo_url>
```

### 2️⃣ Staging all changes  
```sh
git add .
```

### 3️⃣ Committing changes with a message  
```sh
git commit -m "Your commit message"
```

### 4️⃣ Pushing changes to the remote repository  
```sh
git push
```

### 5️⃣ Pulling the latest changes from the `dev` branch  
```sh
git pull origin dev
```

---

## 📖 Explanation

### 🏷️ Branching Strategy
- The project follows a structured branching strategy.
- `main` → Production-ready code.
- `production` → Stable release for production.
- `uat` (User Acceptance Testing) → Testing before deployment.
- `dev` → Active development happens here.
- Developers (`developer1`, `developer2`, `developer3`) work on individual branches inside `dev`.

### 🔄 Workflow
1. Developers clone the repository and switch to their feature branch.
2. They make changes using **VS Code**.
3. Use `git add .` to stage changes.
4. Use `git commit -m "message"` to commit changes.
5. Use `git push` to push changes to their branch.
6. Use `git pull origin dev` to sync with the latest updates.

This structure ensures smooth collaboration and efficient **code management**. 🚀
