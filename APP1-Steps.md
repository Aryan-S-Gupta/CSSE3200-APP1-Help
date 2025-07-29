## Installing Git Bash

**Required for running Git commands on Windows.**

**Download:** [https://git-scm.com/downloads](https://git-scm.com/downloads)

Once installed, open **Git Bash** from the Start Menu or Desktop.

---

## Git User Configuration

Before using Git, configure your global user identity.

### 1. Set Username

```bash
git config --global user.name "your_name"
```

### 2. Set Email

Replace with your actual GitHub email:

```bash
git config --global user.email "your_email@example.com"
```

> **Note:** You must use the same email address that you used to sign up for GitHub.

---

## Check Configuration

```bash
git config --get user.name     # Check Git username
git config --get user.email    # Check Git email
```

---

## Creating a Repository

### A. Initialize Git in an Existing Folder

```bash
git init
```

This command creates a `.git/` folder to track changes in your project.

### B. Clone an Existing GitHub Repository

```bash
git clone [URL]
```

Use either **SSH** or **HTTPS** links from GitHub.

> You can find these links on the GitHub repository page:

![GitHub Clone Options](https://github.com/user-attachments/assets/0b855405-88dc-456e-9fcc-6de46fc9c9eb)

**Example:**

Using HTTPS:

```bash
git clone https://github.com/UQcsse3200/2025-studio-1.git
```

Using SSH:

```bash
git@github.com:UQcsse3200/2025-studio-1.git
```

> **Tip:** SSH is recommended if you’ve set up SSH keys.

---

## Basic File Operations

### 1. Create a New File

```bash
touch filename.txt
```

### 2. View Current Directory

```bash
pwd
```

### 3. View Files and Folders

```bash
ls
```

Use the `-la` flag to include hidden files:

```bash
ls -la
```

### 4. Edit a File

**On Windows (opens in File Explorer):**

```bash
explorer filename.txt
```

**Using a terminal-based editor:**

```bash
vim filename.txt
```

> **Tip:** Use `nano` instead of `vim` if you are new to terminal-based text editors.

---

## Git Workflow Commands

### 1. Add a File to the Staging Area

```bash
git add filename.txt
```

To add all changes:

```bash
git add .
```

### 2. Commit Changes with a Message

```bash
git commit -m "Add initial file"
```

### 3. Pull Latest Changes from GitHub

```bash
git pull
```

Ensure your branch is tracking the appropriate remote branch.

### 4. Push Changes to GitHub

```bash
git push origin main
```

> Replace `main` with your branch name if different.

---

## Helpful Resources

| Task                 | Resource                                                                                                                                           |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| Git Documentation    | [https://git-scm.com/doc](https://git-scm.com/doc)                                                                                                 |
| GitHub Documentation | [https://docs.github.com/en](https://docs.github.com/en)                                                                                           |
| Common Git Issues    | [https://stackoverflow.com/questions/tagged/git](https://stackoverflow.com/questions/tagged/git)                                                   |
| SSH Key Setup        | [https://docs.github.com/en/authentication/connecting-to-github-with-ssh](https://docs.github.com/en/authentication/connecting-to-github-with-ssh) |
| GitHub Student Pack  | [https://education.github.com/pack](https://education.github.com/pack)                                                                             |

---

## Notes

* Use clear and meaningful commit messages.
* Avoid committing large binary files.
* Always pull before pushing to avoid merge conflicts.
* Create branches for new features or bug fixes to keep your main branch clean.
