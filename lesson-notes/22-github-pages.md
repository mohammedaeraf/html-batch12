# Tutorial – Publish a Website Using GitHub Pages

## Introduction

**GitHub Pages** is a service provided by GitHub that allows you to publish a website directly from a GitHub repository.

It is especially useful for hosting **static websites** created using:

* HTML
* CSS
* JavaScript
* Bootstrap
* Images and other frontend files

Once published, your website can be accessed through a URL similar to:

```text
https://username.github.io/repository-name/
```

For example:

```text
https://mohammedaeraf.github.io/webdesign-practice/
```

Your actual URL will depend on your GitHub username and repository name.

---

# Learning Objectives

By the end of this tutorial, you will be able to:

* Upload your website files to a GitHub repository.
* Enable GitHub Pages.
* Select the branch from which the website should be published.
* Access your website using a GitHub Pages URL.

---

# Prerequisites

Before starting, make sure that:

1. You have a GitHub account.
2. You have created a GitHub repository.
3. Your website files have been uploaded to the repository.
4. Your project contains an `index.html` file.

A typical website might look like:

```text
webdesign-practice/
│
├── index.html
├── about.html
├── contact.html
├── style.css
└── images/
    ├── logo.png
    └── banner.jpg
```

### Important

For a basic GitHub Pages website, make sure your main webpage is named:

```text
index.html
```

---

# Step 1 – Upload Your Website Files

First, make sure your latest website files are available in your GitHub repository.

For example:

```text
GitHub Repository
        │
        ├── index.html
        ├── about.html
        ├── style.css
        └── images/
```

If you are using VS Code, you can:

**Source Control → Stage → Commit → Push**

After pushing, open your GitHub repository and verify that the files are visible.

---

# Step 2 – Open Repository Settings

Open your repository on GitHub.

For example:

```text
https://github.com/USERNAME/webdesign-practice
```

Click:

**Settings**

You will find **Settings** in the navigation area of your repository.

> Make sure you are inside the repository. GitHub's account-level settings are different from repository settings.

---

# Step 3 – Select Pages

Inside the repository settings, look for:

**Pages**

Depending on the current GitHub interface, you may find it under:

**Settings → Pages**

The GitHub Pages configuration screen will open.

---

# Step 4 – Select the Branch

Under the GitHub Pages publishing settings, select the branch containing your website.

For a typical project created in this tutorial, select:

```text
Branch: main
```

Then select the appropriate folder, normally:

```text
/ (root)
```

So the configuration will look approximately like:

```text
Source

Branch: main

Folder: / (root)
```

Click:

**Save**

---

# Step 5 – Wait for GitHub Pages to Publish

After clicking **Save**, GitHub will start publishing your website.

It may take a short time for the website to become available.

Usually, students should wait around **30–60 seconds** and then refresh the page.

GitHub may display a message indicating that the site is being deployed.

---

# Step 6 – Open Your Website

Once the deployment is complete, GitHub Pages will provide a website URL.

It will generally follow this pattern:

```text
https://USERNAME.github.io/REPOSITORY-NAME/
```

For example:

```text
https://mohammedaeraf.github.io/webdesign-practice/
```

Click the URL to open your website.

🎉 **Your website is now live on the internet!**

---

# Understanding the Process

The complete process is:

```text
Create Website
      ↓
Upload Files to GitHub
      ↓
Repository Settings
      ↓
Pages
      ↓
Select main Branch
      ↓
Select / (root)
      ↓
Save
      ↓
GitHub Builds & Publishes Website
      ↓
Website is Live
```

---

# What Happens When You Update Your Website?

One of the biggest advantages of GitHub Pages is that you don't have to publish the website manually every time.

Suppose you change:

```text
index.html
```

in VS Code.

You can simply:

```text
Stage
   ↓
Commit
   ↓
Push
```

For example:

```bash
git add .
git commit -m "Updated homepage"
git push
```

GitHub Pages will detect the updated files and deploy the latest version.

After the deployment finishes, refresh your website.

---

# Important: File Paths

When publishing a website, make sure your file paths work correctly.

For example:

```html
<img src="images/logo.png">
```

is preferable to:

```html
<img src="C:\Users\Ahmed\Desktop\website\images\logo.png">
```

Your website must use **relative paths** for local project files.

Similarly:

```html
<link rel="stylesheet" href="style.css">
```

is appropriate.

---

# Common Problems

## 1. Website Does Not Open

Check that your repository contains:

```text
index.html
```

GitHub Pages looks for your website's entry point based on the publishing configuration.

---

## 2. CSS Is Not Working

Check the CSS path.

For example:

```html
<link rel="stylesheet" href="style.css">
```

If your CSS is inside a folder:

```html
<link rel="stylesheet" href="css/style.css">
```

---

## 3. Images Are Not Displaying

Check the image path:

```html
<img src="images/photo.jpg">
```

Make sure:

* The image exists.
* The folder name is correct.
* The filename is correct.
* The file extension is correct.

---

## 4. Website Looks Different From Your Local Computer

Check whether you have:

* Pushed the latest changes to GitHub.
* Used correct relative paths.
* Included all required CSS and JavaScript files.
* Used HTTPS-compatible external resources.

For example, CDN resources should generally use:

```text
https://
```

rather than:

```text
http://
```

---

# Mini Practice Exercise

## Publish Your Web Design Project

Take one of your existing Bootstrap projects and publish it using GitHub Pages.

### Requirements

* [ ] Create a GitHub repository.
* [ ] Upload your website files.
* [ ] Make sure `index.html` exists.
* [ ] Open **Settings**.
* [ ] Select **Pages**.
* [ ] Select the `main` branch.
* [ ] Select `/ (root)`.
* [ ] Click **Save**.
* [ ] Wait for the website to be published.
* [ ] Open your GitHub Pages URL.
* [ ] Verify that the website works correctly.

### Expected Result

Your website should be accessible through a URL similar to:

```text
https://yourusername.github.io/your-repository/
```

---

# Quick Revision

### To publish a website:

```text
1. Upload files
       ↓
2. Settings
       ↓
3. Pages
       ↓
4. Select main branch
       ↓
5. Select / (root)
       ↓
6. Save
       ↓
7. Wait for deployment
       ↓
8. Open GitHub Pages URL
```

## Key Point

**GitHub** stores your website code.

**GitHub Pages** publishes that code as a website.

```text
GitHub Repository
       ↓
GitHub Pages
       ↓
Live Website 🌐
```
