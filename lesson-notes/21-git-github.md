Here is a student-friendly tutorial version, keeping the workflow simple and focused on what you taught today.

# Tutorial – Git & GitHub: Creating a Repository and Uploading Files

## Introduction

**Git** and **GitHub** are commonly used by web designers and developers to store, manage, and share their projects.

In this tutorial, we will learn how to:

* Install Git on our computer
* Create a GitHub account
* Configure Git
* Create a repository on GitHub
* Create a local Git repository
* Connect the local repository to GitHub
* Upload/push website files to GitHub

---

# Part A – Prerequisites

## Step 1 – Install Git

Git is the software that allows us to manage our project using version control.

Download Git from the official website:

[Download Git](https://git-scm.com/install/?utm_source=chatgpt.com)

Install Git using the default installation options.

### Verify Installation

After installation, open **Git Bash** and run:

```bash
git --version
```

If Git is installed correctly, you should see something similar to:

```text
git version 2.x.x
```

The exact version number may be different.

---

# Step 2 – Sign Up on GitHub

GitHub is an online platform where we can store and share Git repositories.

Visit:

[GitHub](https://github.com/?utm_source=chatgpt.com)

Click **Sign up** and create your account.

You can register using your email address and follow the verification steps provided by GitHub.

> **Tip:** Choose a professional GitHub username because it can become part of your developer portfolio.

For example:

```text
mohammedaeraf
johnsmith
johnsmith-dev
```

---

# Step 3 – Sign In to GitHub

After creating your account:

1. Open GitHub.
2. Click **Sign in**.
3. Enter your GitHub credentials.
4. You should now see your GitHub dashboard.

---

# Step 4 – Configure Git

Before using Git for the first time, configure your **username** and **email address**.

Open **Git Bash** and run:

```bash
git config --global user.name "mohammedaeraf"
```

Then configure your email:

```bash
git config --global user.email "aeraf@outlook.com"
```

### Important

Students should replace these values with **their own name/username and email**.

For example:

```bash
git config --global user.name "John Smith"
```

```bash
git config --global user.email "john@example.com"
```

### Why do we configure this?

Git uses this information to identify who made a particular commit.

---

# Part B – Create a Repository and Upload Files

Now let's upload a website project to GitHub.

Suppose we have a local project called:

```text
webdesign-practice
```

It may contain:

```text
webdesign-practice
│
├── index.html
├── about.html
├── contact.html
├── css/
│   └── style.css
└── images/
    └── logo.png
```

---

# Step 1 – Create a Repository on GitHub

Sign in to GitHub.

Click:

**+ → New repository**

Enter a repository name.

For example:

```text
webdesign-practice
```

You can optionally add a description:

```text
Web Design practice projects
```

Choose whether the repository should be:

* **Public** – anyone can view it
* **Private** – only you and authorized users can view it

For student practice projects, **Public** is often useful for building a portfolio.

Then click:

**Create repository**

---

# Step 2 – Copy the Repository URL

After creating the repository, GitHub will provide a URL similar to:

```text
https://github.com/USERNAME/webdesign-practice.git
```

For example:

```text
https://github.com/mohammedaeraf/webdesign-practice.git
```

> **Important:** Students must use their **own GitHub username** in the URL.

---

# Step 3 – Open the Local Project

Open the folder containing your website project.

For example:

```text
Documents
   └── webdesign-practice
```

Open **Git Bash** inside this folder.

You can usually do this by:

**Right-click → Open Git Bash Here**

---

# Step 4 – Initialize the Local Repository

Run:

```bash
git init
```

This initializes Git inside your project folder.

You may see a message similar to:

```text
Initialized empty Git repository
```

Git has now started tracking this project.

Conceptually:

```text
Website Folder
      ↓
   git init
      ↓
Local Git Repository
```

---

# Step 5 – Connect the Local Repository to GitHub

Now we need to tell Git where the online GitHub repository is located.

Run:

```bash
git remote add origin https://github.com/USERNAME/webdesign-practice.git
```

For example:

```bash
git remote add origin https://github.com/mohammedaeraf/webdesign-practice.git
```

Here:

```text
origin
```

is the name we give to the remote GitHub repository.

Think of it as:

```text
Local Repository
       │
       │ origin
       ↓
GitHub Repository
```

---

Yes. For beginners, I actually recommend using **VS Code's Source Control (SCM)** for Steps 6–8. It makes the concepts of **Stage → Commit → Push** much easier to visualize.

You can replace Steps 6, 7 and 8 with the following:

---

# Step 6 – Stage Your Files Using VS Code

Open your project folder in **VS Code**.

On the left side, click the **Source Control** icon:

**Source Control (SCM) → Branch icon**

You should see your project files under **Changes**.

For example:

```text
CHANGES

M index.html
M about.html
M contact.html
? css/style.css
? images/logo.png
```

### Stage All Files

Click the **`+`** button next to **Changes**.

This stages all the files.

The files will move from:

```text
Changes
```

to:

```text
Staged Changes
```

### What does "Stage" mean?

Staging means:

> **Select the changes that you want to include in the next commit.**

You can think of it as preparing your files for saving.

```text
Files
  ↓
Changes
  ↓
Stage (+)
  ↓
Staged Changes
```

---

# Step 7 – Commit Your Changes Using VS Code

After staging the files, look at the **Source Control** panel.

At the top, you will see a box for entering a commit message.

Enter:

```text
Initial website
```

Then click:

**Commit**

Alternatively, you may see a button such as:

**Commit**

or a **✓ checkmark** at the top of the Source Control panel.

Your staged changes will now be saved as a Git commit.

### What is a Commit?

A commit is a **saved snapshot of your project changes**.

For example:

```text
Initial website
```

Later, you might make another change and create:

```text
Added Bootstrap navbar
```

Then:

```text
Updated contact form
```

A project's Git history may therefore look like:

```text
Initial website
      ↓
Added Bootstrap navbar
      ↓
Updated contact form
      ↓
Added footer
```

---

# Step 8 – Push Your Files to GitHub Using VS Code

After committing your changes, we need to upload them to GitHub.

In the VS Code Source Control panel, look for:

**Sync Changes**

or:

**Publish Branch**

If this is the **first time** you're uploading the project, you may see:

**Publish Branch**

Click it.

VS Code will connect your local repository to GitHub and push your project.

If the repository has already been connected, you will normally see:

**Sync Changes**

Click it to synchronize your local repository with GitHub.

You can also use:

**Source Control → `...` → Push**

---

## What Happens?

The files are uploaded from:

```text
VS Code
   ↓
Local Git Repository
   ↓
GitHub
```

# Step 9 – Check Your GitHub Repository

Open your GitHub repository in the browser.

For example:

```text
https://github.com/USERNAME/webdesign-practice
```

Refresh the page.

You should now see your project files:

```text
webdesign-practice
│
├── index.html
├── about.html
├── contact.html
├── css/
└── images/
```

🎉 **Congratulations! Your local website project has been uploaded to GitHub.**

---
Go to your GitHub repository and refresh the page.

You should now see your project files.

---

# The Complete VS Code Workflow


```text
          VS CODE
             │
             ↓
       Create Website
             │
             ↓
       Source Control
             │
             ↓
       Stage Changes (+)
             │
             ↓
          Commit
             │
             ↓
      Publish / Push
             │
             ↓
          GITHUB
```

### In simple words:

**Stage → Commit → Push**

```text
Stage
"Which files do I want to save?"

       ↓

Commit
"Save a snapshot of these changes."

       ↓

Push
"Upload those changes to GitHub."
```

---