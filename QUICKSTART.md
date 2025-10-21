# ⚡ Quick Start Guide

## Deploy in 5 Minutes

### 1️⃣ Create Repository
Go to https://github.com/new and create:
- Name: `cwarre33.github.io`
- Public: ✓
- Click "Create"

### 2️⃣ Push Code
```bash
cd C:\Users\camwa\DevEnvironment\contributions-portfolio
git remote add origin https://github.com/cwarre33/cwarre33.github.io.git
git branch -M main
git push -u origin main
```

### 3️⃣ Enable Pages
- Go to Repository Settings
- Scroll to "Pages"
- Select "main" branch
- Click "Save"

### 4️⃣ Done! 🎉
Visit: https://cwarre33.github.io

---

## Files Overview

| File | What It Is | Audience |
|------|-----------|----------|
| `index.html` | Your portfolio page | Employers, recruiters, visitors |
| `README.md` | Detailed information | Developers, technical folks |
| `contributions.json` | Raw data | APIs, tools, automation |
| `DEPLOYMENT.md` | Full setup guide | You (if troubleshooting) |

---

## Customization

### Update a PR Status to "Merged"
Edit `contributions.json`, find the PR, change:
```json
"status": "in_review"
```
to:
```json
"status": "merged"
```

### Update Contact Info
Edit `README.md`:
- Replace my email with yours
- Update social links

### Change Colors
Edit `index.html`, find this section:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```
Change to your preferred hex colors!

---

## Share Your Portfolio

✅ Link in GitHub bio
✅ LinkedIn projects section
✅ Resume/CV
✅ Email signature
✅ Portfolio websites

---

## Support

- Full guide: See `DEPLOYMENT.md`
- Repo: https://github.com/cwarre33/cwarre33.github.io
- GitHub Pages docs: https://pages.github.com

---

**You've got this!** 🚀
