## 📦 Installing Git Bash

**Required for running Git commands on Windows.**

🔗 Download: [https://git-scm.com/downloads](https://git-scm.com/downloads)

Once installed, open **Git Bash** from the Start Menu or Desktop.

---

## 👤 Git User Configuration

Before using Git, set your global user identity.

### 1. Set Username

```bash
git config --global user.name "your_name"
```

### 2. Set Email

Replace with your actual GitHub email.

```bash
git config --global user.email "your_email@example.com"
```

> 💡 You must use the same email you used for signing up on GitHub.

---

## 🔍 Check Configuration

```bash
git config --get user.name     # Check Git username
git config --get user.email    # Check Git email
```

---

## 📁 Creating a Repository

### 🅰️ A. Initialize Git in an Existing Folder

```bash
git init
```

This creates a `.git/` folder to track changes.

### 🅱️ B. Clone an Existing GitHub Repository

```bash
git clone [URL]
```

Use **SSH** or **HTTPS** links from GitHub.

📌 Example:

```bash
git clone https://github.com/uq-csse3200/sample-project.git
```

> 💡 SSH is recommended if you’ve set up SSH keys.

---

## 📄 Basic File Operations

### 1. Create a New File

```bash
touch filename.txt
```

Alternative (Windows):

```bash
echo. > filename.txt
```

### 2. View Current Directory

```bash
pwd
```

### 3. View Files and Folders

```bash
ls
```

Use `ls -la` to see hidden files (like `.git/`).

### 4. Edit a File

* On Windows:

```bash
explorer filename.txt
```

* Using terminal editor:

```bash
vim filename.txt
```

> Tip: Use `nano` instead of `vim` if you're new to terminal editing.

---

## 💾 Git Workflow Commands

### 1. Add a File to Staging Area

```bash
git add filename.txt
```

To add all changes:

```bash
git add .
```

### 2. Commit Changes with Message

```bash
git commit -m "Add initial file"
```

### 3. Pull Latest Changes from GitHub

```bash
git pull
```

Make sure your branch is tracking the remote branch.

### 4. Push Changes to GitHub

```bash
git push origin main
```

> Replace `main` with your branch name if different.

---

## 🆘 Helpful Resources

| Task                | Resource                                                                                                                                           |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| Git Docs            | [https://git-scm.com/doc](https://git-scm.com/doc)                                                                                                 |
| GitHub Docs         | [https://docs.github.com/en](https://docs.github.com/en)                                                                                           |
| Common Git Errors   | [https://stackoverflow.com/questions/tagged/git](https://stackoverflow.com/questions/tagged/git)                                                   |
| SSH Key Setup       | [https://docs.github.com/en/authentication/connecting-to-github-with-ssh](https://docs.github.com/en/authentication/connecting-to-github-with-ssh) |
| GitHub Student Pack | [https://education.github.com/pack](https://education.github.com/pack)                                                                             |

---

## 🧾 Notes

* Use meaningful commit messages.
* Avoid committing large binaries.
* Always pull before pushing to avoid conflicts.
* Branch often for features or bug fixes.
