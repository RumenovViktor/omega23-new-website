# How to Deploy Omega23 Website to GitHub Pages

This guide will walk you through the steps to deploy your new website to GitHub Pages.

## Prerequisites
- A GitHub account.
- Git installed on your computer.

## Step 1: Initialize Git
Open your terminal in the project folder (`/Users/viktorrumenov/Documents/Development/omega23website`) and run:

```bash
git init
```

## Step 2: Create a Repository on GitHub
1. Go to [GitHub.com](https://github.com) and log in.
2. Click the **+** icon in the top right and select **New repository**.
3. Name your repository (e.g., `omega23-website`).
4. Make sure it is **Public** (required for free GitHub Pages).
5. Click **Create repository**.

## Step 3: Push Your Code
Back in your terminal, run the following commands (replace `YOUR_USERNAME` with your actual GitHub username):

```bash
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/omega23-website.git
git push -u origin main
```

## Step 4: Enable GitHub Pages
1. Go to your repository page on GitHub.
2. Click on **Settings** (top tab).
3. On the left sidebar, click on **Pages**.
4. Under **Build and deployment** > **Source**, select **Deploy from a branch**.
5. Under **Branch**, select `main` and `/ (root)`.
6. Click **Save**.

## Step 5: View Your Website
- GitHub will take a minute or two to build your site.
- Refresh the Pages settings page. You will see a message: "Your site is live at..." with a link.
- Click the link to view your live website!

## Updating Your Site
Whenever you make changes to the code:
1. Save your files.
2. Run:
   ```bash
   git add .
   git commit -m "Description of changes"
   git push
   ```
3. GitHub Pages will automatically update with your new changes.
