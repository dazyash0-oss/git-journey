
---

# 🚀 Git & GitHub Course Notes

Welcome to the ultimate cheat sheet for Git and GitHub! This repository serves as a practical guide to understanding version control, managing repositories, and collaborating with others.

---

## 📌 1. Version Control Basics

**Version Control Systems (VCS)** track changes to files over time, allowing you to recall specific versions later.

* **Git**: A local, decentralized version control system. It lives on your computer and tracks your project's history.
* **GitHub**: A cloud-based hosting service for Git repositories. It lets you share your code, collaborate with others, and back up your work.

---

## 💻 2. Essential Git Commands

Here is the typical workflow for managing a project locally:

### ⚙️ Configuration & Setup

Before doing anything else, set up your identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

```

### 🛠️ Initializing & Staging

* **`git init`**: Turns your current directory into a brand-new Git repository.
* **`git status`**: Shows the state of your working directory (tracked vs. untracked files).
* **`git add <filename>`**: Moves a specific file to the **Staging Area**.
* **`git add .`**: Stages *all* modified and new files in the current folder.

### 💾 Committing Changes

* **`git commit -m "Your descriptive message"`**: Takes a snapshot of your staged changes and saves it permanently to the project history.

---

## 🌿 3. Branching & Merging

Branches allow you to work on new features or fix bugs without messing up the main project code.

* **`git branch`**: Lists all the branches in your repository.
* **`git branch <branch-name>`**: Creates a new branch.
* **`git checkout <branch-name>`** (or **`git switch <branch-name>`**): Switches to that branch.
* **`git checkout -b <branch-name>`**: Shortcut to create *and* switch to a new branch instantly.
* **`git merge <branch-name>`**: Merges the specified branch's history into your current active branch.

---

## ☁️ 4. Working with GitHub (Remote Repositories)

Once your code is tracked locally, you use GitHub to share it.

| Command | What it Does |
| --- | --- |
| **`git remote add origin <URL>`** | Links your local repository to a remote GitHub repository. |
| **`git push -u origin main`** | Pushes your local commits to GitHub (and remembers the path for next time). |
| **`git clone <URL>`** | Copies an existing GitHub repository onto your local computer. |
| **`git pull`** | Fetches the latest changes from GitHub and integrates them into your local project. |

---

## 🤝 5. The GitHub Collaboration Workflow

When working with a team or contributing to Open Source, follow this standard pattern:

1. **Fork** the repository (creates your own copy of their project on GitHub).
2. **Clone** your fork to your local machine.
3. Create a new **Feature Branch** (`git checkout -b new-feature`).
4. Make your changes, `git add`, and `git commit` them.
5. **Push** the branch to *your* GitHub fork (`git push origin new-feature`).
6. Open a **Pull Request (PR)** on GitHub to ask the original project owner to merge your changes.

---

## 🔀 6. Fixing Mistakes (Quick Reference)

* **Undo `git add` (before committing):**
```bash
git restore --staged <filename>

```


* **Modify the last commit message:**
```bash
git commit --amend -m "New and improved message"

```


* **Discard local changes to a file (revert to last commit):**
```bash
git restore <filename>

```
### for revision 

https://docs.chaicode.com/youtube/chai-aur-git/introduction/

