# Setup: Deploy to GitHub Pages

## Step 1: Create the GitHub repository

1. Go to https://github.com/new
2. **Repository name:** `presence-ledger`
3. **Description:** "NZ citizenship presence requirement planner"
4. **Public:** Yes
5. **Do NOT** initialize with README (we already have one)
6. Click **Create repository**

## Step 2: Initialize git and push from your local machine

Open your terminal in this folder and run:

```bash
# Configure git (one-time setup if you haven't already)
git config --global user.email "your.email@example.com"
git config --global user.name "Your Name"

# Initialize the repo
git init
git branch -m main

# Add GitHub remote (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/presence-ledger.git

# Add all files and commit
git add .
git commit -m "Initial commit: Presence Ledger app"

# Push to GitHub
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repo: `https://github.com/YOUR_USERNAME/presence-ledger`
2. Click **Settings** → **Pages** (left sidebar)
3. Under "Build and deployment":
   - **Source:** "Deploy from a branch"
   - **Branch:** `main`, folder: `/ (root)`
4. Click **Save**

GitHub will deploy in ~30 seconds. Your app will be live at:

```
https://YOUR_USERNAME.github.io/presence-ledger/
```

## Files in this folder

- **index.html** — The app (open locally in a browser to test)
- **README.md** — Full documentation for the GitHub repo
- **.gitignore** — Standard ignores for Node/build files
- **SETUP.md** — This file

## What's included

- ✅ Single-file HTML app (no build process)
- ✅ Completely client-side (no backend needed)
- ✅ Works offline
- ✅ Data stored in browser only
- ✅ Ready to deploy anywhere

Just follow the steps above and you're done!
