# Developer Portal Demo

## Overview

This *Developer Documentation Portal* demo was built with **[MkDocs](https://www.mkdocs.org/)** and using the **Material for MkDocs** theme.

This repository is ideal for anyone learning to build and host developer-facing documentation sites using a **Docs-as-Code** approach and showcasing ***technical documentation best practices for APIs, release notes,*** and ***onboarding tutorials***. 

This allows technical writers and developers to collaborate using the same tools and workflows as engineers.

Live demo: **https://prineetkaur.github.io/Developer-Portal-Demo/**

---
## Project Preview

![Preview of Developer Portal Demo](Preview.png)

---

## How This Repo Is Organized

- **main branch** → contains the source Markdown files and MkDocs configuration.  
- **gh-pages branch** → is automatically created by MkDocs to host the static site.  

---

## Folder Structure

```
Developer-Portal-Demo/
├── docs/
│   ├── index.md              # Home page
│   ├── getting-started.md    # Getting started guide
│   ├── payments.md           # Example API documentation
│   ├── release-notes.md      # Release notes example
│   └── tutorials/
│       └── tutorial1.md      # Tutorial example
├── mkdocs.yml                # MkDocs configuration
└── README.md                 # This file
```

---

## Workflow Summary
1. Write docs in Markdown (`.md` files) inside the `docs/` folder.  
2. Configure layout and navigation in `mkdocs.yml`.  
3. Run `mkdocs serve` for local preview.  
4. Deploy to GitHub Pages using `mkdocs gh-deploy`.

MkDocs automatically builds the static site and pushes it to your repository’s `gh-pages` branch for hosting.

---

## How to Run Locally

### 1️⃣ Install Python

Ensure **Python 3.8+** is installed:
```bash
python --version
```

### 2️⃣ Install MkDocs and Theme
```bash
pip install mkdocs mkdocs-material
```
You can also verify if MkDocs is already installed using:
```bash
mkdocs --version
```
If you see a version number, MkDocs is installed correctly.

### 3️⃣ Clone the Repository
```bash
git clone https://github.com/PrineetKaur/Developer-Portal-Demo.git
cd Developer-Portal-Demo
```

### 4️⃣ Serve Locally
Start the documentation site locally to preview changes:
```bash
mkdocs serve
```
Then open your browser at:  
👉 **http://127.0.0.1:8000**

### 5️⃣ Build Static Files
To generate the static HTML output:
```bash
mkdocs build
```
This generates a `site/` folder containing the compiled HTML files.

### 6️⃣ Initialize Git and Push to GitHub

If you’re setting up this project for the first time (for example, from a zip download or after copying the folder), you’ll need to initialize a Git repository and connect it to your own GitHub repo before deployment. Follow the commands below to do so:

```bash
# Initialize Git
git init

# Add all project files
git add.

# Commit files
git commit -m "Initial commit: Demo Developer Portal"

# Link to your own GitHub repository
git remote add origin https://github.com/YOUR_USERNAME/demo-dev-portal.git

# Rename default branch to main
git branch -M main

# Push all files to GitHub
git push -u origin main
```

### 7️⃣ Deploy to GitHub Pages
Once your code is on GitHub, run the following from your project folder:
```bash
mkdocs gh-deploy
```
Use the above to deploy and even update every time you make any changes in your content pages or add more pages. Simply re-run the above command, and it will rebuild and update your live documentation automatically.

Your live site will be published automatically at:  
👉 **https://YOUR_Username.github.io/Developer-Portal-Demo/**


## 8️⃣ Verify Deployment

1. Go to your repository on GitHub → **Settings → Pages**
2. Under *Branch*, ensure the following is set:

```
gh-pages / (root)
```

3. Wait 1–2 minutes, then open your live site URL.

---

## Credits

Built with ❤️ using [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).  
Created by [Prineet Kaur](https://github.com/PrineetKaur) as part of a documentation and developer advocacy learning project.
