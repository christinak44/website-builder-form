# Quick Setup Guide

## Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **+** icon → **New repository**
3. Name it: `website-builder-form`
4. Make it **Public** (required for free GitHub Pages)
5. **Don't** initialize with README, .gitignore, or license
6. Click **Create repository**

## Step 2: Push Files to GitHub

Run these commands in the `form-repo` directory:

```bash
cd form-repo

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Website Builder form"

# Add your GitHub repo (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/website-builder-form.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **Save**
5. Wait 1-2 minutes for GitHub to build

## Step 4: Access Your Form

Your form will be available at:
- **Landing page:** `https://YOUR_USERNAME.github.io/website-builder-form/`
- **Direct form:** `https://YOUR_USERNAME.github.io/website-builder-form/website-builder-form.html`

## Step 5: Share!

Copy the link and share it with clients via email, your website, or social media.
