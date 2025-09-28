# Git Instructions for rsschool-cv project

## Step 1: Initialize repository
```bash
git init
git add README.md
git commit -m "init: add README.md"
```

## Step 2: Connect to GitHub
1. Create repository on GitHub named `rsschool-cv`
2. Connect local repository to GitHub:
```bash
git remote add origin https://github.com/AlanKowalzky/rsschool-cv.git
git branch -M main
git push -u origin main
```

## Step 3: Create gh-pages branch
```bash
git checkout -b gh-pages
```

## Step 4: Add CV files (execute in gh-pages branch)
```bash
git add cv.md
git commit -m "feat: add CV content in markdown format"

# Update README.md with proper link
git add README.md
git commit -m "docs: update README with CV link"

# Add more commits if needed (minimum 3 in gh-pages)
git add .
git commit -m "refactor: improve CV formatting and content"
```

## Step 5: Push to GitHub
```bash
git push -u origin gh-pages
```

## Step 6: Create Pull Request
1. Go to GitHub to your repository
2. Create Pull Request from `gh-pages` to `main`
3. Title: "Markdown & Git"
4. Description according to template:
   - Deployed to GitHub Pages: https://AlanKowalzky.github.io/rsschool-cv/cv
   - Pull Request: link to PR
   - Task: Markdown & Git

## Step 7: Activate GitHub Pages
1. In repository settings enable GitHub Pages
2. Select `gh-pages` branch as source
3. Check if CV is available at: https://AlanKowalzky.github.io/rsschool-cv/cv

## Important notes:
- DO NOT merge Pull Request
- Make sure you have minimum 3 commits in gh-pages branch
- Use commit prefixes: init:, feat:, fix:, refactor:, docs:
- Username AlanKowalzky is already set in links