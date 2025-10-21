# 🚀 Deployment Guide - GitHub Pages

This guide will walk you through deploying your contributions portfolio to GitHub Pages at `https://cwarre33.github.io`

## Prerequisites

- GitHub account (already set up with username: `cwarre33`)
- Git installed locally (you already have this)
- The portfolio files in `C:\Users\camwa\DevEnvironment\contributions-portfolio\`

## Step-by-Step Deployment

### Step 1: Create a New GitHub Repository

1. Go to [GitHub](https://github.com/new)
2. Create a new repository with these exact settings:
   - **Repository name**: `cwarre33.github.io`
   - **Description**: "Open Source Contributions Portfolio"
   - **Public**: Yes (required for GitHub Pages)
   - **Add .gitignore**: No (we already have one)
   - **Add README**: No (we already have one)

### Step 2: Add Remote and Push

In your terminal:

```bash
cd C:\Users\camwa\DevEnvironment\contributions-portfolio

# Add your GitHub repository as the remote
git remote add origin https://github.com/cwarre33/cwarre33.github.io.git

# Verify the remote was added
git remote -v

# Push to GitHub (this will create the main branch if needed)
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository: https://github.com/cwarre33/cwarre33.github.io
2. Click **Settings** (in the repository menu)
3. Scroll down to **Pages** section
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

GitHub will automatically deploy your site!

### Step 4: Verify Deployment

After a few seconds, GitHub will build your site. You should see:

```
✓ Your site is live at https://cwarre33.github.io
```

Visit your portfolio at: **https://cwarre33.github.io**

## 📝 Making Updates

After you make changes to your contributions (e.g., when a PR gets merged):

```bash
cd C:\Users\camwa\DevEnvironment\contributions-portfolio

# Edit the files you want to change
# For example, update contributions.json or index.html

# Commit your changes
git add -A
git commit -m "Update: Changed contribution status to merged"

# Push to GitHub
git push origin main
```

GitHub will automatically rebuild your site with the new changes!

## 🎨 Customization Options

### Update Contribution Status

Edit `contributions.json` and change `"status"` from:
- `"in_review"` → `"merged"` (when PR is accepted)
- Update the badge accordingly in `index.html`

### Update Impact Numbers

In `index.html`, update the stats section:

```html
<div class="stat-number">X</div>  <!-- Change to your numbers -->
```

### Add Social Links

In `_config.yml`, update social links:

```yaml
social_links:
  github: cwarre33
  linkedin: your-linkedin-username
  twitter: your-twitter-handle
```

## 🔗 Share Your Portfolio

Once deployed, you can share it:

- **Direct Link**: https://cwarre33.github.io
- **Add to GitHub Profile**: Edit your GitHub profile bio or README
- **LinkedIn**: Add to your projects section
- **Resume**: Include the URL
- **Email Signature**: Add a link to your portfolio

## 📊 Portfolio Contents

Your portfolio includes:

| File | Purpose |
|------|---------|
| `index.html` | Main showcase page (public-facing) |
| `README.md` | Detailed descriptions and learnings |
| `contributions.json` | Machine-readable contribution data |
| `_config.yml` | Jekyll configuration for GitHub Pages |
| `.gitignore` | Git ignore patterns |

## ✅ Verification Checklist

- [ ] Repository created at `cwarre33.github.io`
- [ ] All files pushed to GitHub main branch
- [ ] GitHub Pages enabled in repository settings
- [ ] Site live at https://cwarre33.github.io
- [ ] All links working (click to verify PRs load)
- [ ] Mobile responsive (test on phone)
- [ ] Social links configured in `_config.yml`

## 🐛 Troubleshooting

### Site not showing up?
- Wait 2-3 minutes for GitHub to build
- Check repository settings → Pages for build status
- Ensure branch is set to `main` in Pages settings

### Links not working?
- Verify all PR numbers and URLs in `index.html`
- Check that PR numbers match actual GitHub PR URLs

### Styling looks broken?
- Clear browser cache (Ctrl+Shift+Delete)
- Try a different browser to isolate issues

## 🎉 You're All Set!

Your open-source contributions are now showcased professionally online!

### Next Steps:

1. ✅ Deploy to GitHub Pages
2. ✅ Share with community/employers
3. ✅ Update when PRs get merged
4. ✅ Continue making awesome contributions!

---

**Need help?** Check GitHub Pages documentation: https://pages.github.com/
