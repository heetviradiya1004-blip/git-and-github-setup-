# Git & GitHub Setup Guide (Windows)

## 1. Install Git

Download and install Git from:
https://git-scm.com/install/windows

---

## 2. Open Git Bash

After installing Git, open **Git Bash**.

---

## 3. Configure Your Git Account

If you want to remove any existing Git account configuration, run:

```bash
git config --global --unset user.name
git config --global --unset user.email
```

Now set your Git username and email:

```bash
git config --global user.name "heetviradiya1004-blip"
git config --global user.email "heetviradiya1004@gmail.com"
```

---

## 4. Verify Your Git Configuration

Run:

```bash
git config --list
```

Check that your **user.name** and **user.email** are correct.

---

## 5. Create Your Project Folder

Example:

```
News-Website
```

Open this folder in **Visual Studio Code**.

---

## 6. Create a New Repository on GitHub

1. Sign in to GitHub.
2. Click the **New** (green) button.
3. Enter a repository name (e.g., `news-website`).
4. Click **Create repository**.

---

## 7. Connect Your Local Project to GitHub

Open the VS Code terminal and initialize Git:

```bash
git init
```

Copy the **git remote add origin** command from GitHub and run it.

Example:

```bash
git remote add origin https://github.com/username/news-website.git
```

---

## 8. Check Your Current Branch

Run:

```bash
git branch
```

If needed, rename your branch to `main`:

```bash
git branch -M main
```

---

## 9. Upload Your Project

Run these commands one by one:

```bash
git add .
git commit -m "Initial commit"
git push -u origin main
```

> Replace **main** with your current branch name if it is different.

---

# Daily Workflow

Whenever you make changes to your project:

```bash
git add .
git commit -m "Describe your changes"
git push origin main
```

Example:

```bash
git add .
git commit -m "Added login page"
git push origin main
```

Repeat this workflow every time you edit, add, or delete files.

---

## Useful Git Commands

Check status:

```bash
git status
```

View commit history:

```bash
git log
```

Check remote repository:

```bash
git remote -v
```

Check current branch:

```bash
git branch
```

View Git configuration:

```bash
git config --list
```
