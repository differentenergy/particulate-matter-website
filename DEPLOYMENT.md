# GitHub Deployment Guide

Follow these steps to deploy your website to GitHub Pages:

## Step 1: Create a GitHub Account
If you don't have one already, go to https://github.com and sign up.

## Step 2: Create a New Repository

1. Go to https://github.com/new
2. Repository name: `particulate-matter-website` (or any name you prefer)
3. Description: "Interactive bilingual website about particulate matter and air quality"
4. Set to **Public** (required for free GitHub Pages)
5. **DO NOT** check "Initialize with README" (we already have one)
6. Click "Create repository"

## Step 3: Upload Your Files

### Option A: Using GitHub Web Interface (Easiest)

1. On your new repository page, click "uploading an existing file"
2. Drag and drop all files from the `particulate-matter-website` folder:
   - `index.html`
   - `README.md`
   - `.gitignore`
3. Add commit message: "Initial commit"
4. Click "Commit changes"

### Option B: Using Git Command Line

If you have Git installed on your computer:

```bash
# Navigate to the project folder
cd /path/to/particulate-matter-website

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit: Interactive particulate matter website"

# Add GitHub as remote (replace YOUR-USERNAME and YOUR-REPO-NAME)
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** (top right)
3. Scroll down and click **Pages** in the left sidebar
4. Under "Source":
   - Select branch: **main**
   - Select folder: **/ (root)**
5. Click **Save**
6. Wait 1-2 minutes for deployment

## Step 5: Access Your Live Website

Your site will be available at:
```
https://YOUR-USERNAME.github.io/particulate-matter-website
```

GitHub will show you the exact URL in the Pages settings.

## Step 6: Update Your Website (Future Changes)

### Using GitHub Web Interface:
1. Navigate to the file you want to edit
2. Click the pencil icon (Edit)
3. Make changes
4. Commit changes
5. Wait ~1 minute for automatic redeployment

### Using Git Command Line:
```bash
# Make your changes to files
# Then:
git add .
git commit -m "Description of your changes"
git push
```

## Troubleshooting

**Site not loading?**
- Wait 2-3 minutes after enabling Pages
- Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Check that repository is Public
- Verify index.html is in root directory

**Changes not showing?**
- GitHub Pages can take 1-2 minutes to update
- Clear browser cache
- Try incognito/private browsing mode

## Custom Domain (Optional)

To use your own domain (e.g., particulates.com):
1. Buy a domain from any registrar
2. In GitHub repository Settings > Pages, add your custom domain
3. In your domain registrar, add CNAME record pointing to: `YOUR-USERNAME.github.io`
4. Wait for DNS propagation (up to 24 hours)

## Need Help?

- GitHub Pages Documentation: https://docs.github.com/en/pages
- GitHub Support: https://support.github.com
