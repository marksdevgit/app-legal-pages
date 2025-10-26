# Quick Start Guide

## 🎯 What You Have

A complete set of legal pages for **SuperFusionGrid** and **Shelfwise**, ready to deploy for App Store submission.

## ✅ SuperFusionGrid - READY TO DEPLOY

All three pages are complete and comprehensive:
- ✅ Privacy Policy (complete)
- ✅ Terms of Service (complete)
- ✅ Support Page (complete)

**Before deploying, just replace:**
1. `[YOUR EMAIL HERE]` with your support email
2. `[YOUR JURISDICTION]` with your legal jurisdiction (e.g., "California, USA")

## ⚠️ Shelfwise - NEEDS CUSTOMIZATION

Template pages with TODO markers - you'll need to fill in details about:
- What data Shelfwise collects
- Third-party services it uses
- Features and functionality
- Backup/sync capabilities

## 🚀 Deploy in 5 Minutes

### Step 1: Create GitHub Repository
1. Go to [github.com](https://github.com) and click "New repository"
2. Name it `app-legal-pages` (or any name you prefer)
3. Make it **Public** (required for GitHub Pages)
4. Don't initialize with README (we already have one)
5. Click "Create repository"

### Step 2: Push to GitHub
```bash
cd /Users/markbridge/Documents/app-legal-pages
git init
git add .
git commit -m "Initial commit: Add legal pages for apps"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/app-legal-pages.git
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings** (top right)
3. Scroll down to **Pages** (left sidebar)
4. Under "Source", select **main** branch
5. Click **Save**
6. Wait 2-3 minutes for deployment

### Step 4: Get Your URLs
Your pages will be live at:
```
https://YOUR-USERNAME.github.io/app-legal-pages/
```

**For SuperFusionGrid:**
- Privacy: `https://YOUR-USERNAME.github.io/app-legal-pages/superfusiongrid/privacy.html`
- Terms: `https://YOUR-USERNAME.github.io/app-legal-pages/superfusiongrid/terms.html`
- Support: `https://YOUR-USERNAME.github.io/app-legal-pages/superfusiongrid/support.html`

**For Shelfwise:**
- Privacy: `https://YOUR-USERNAME.github.io/app-legal-pages/shelfwise/privacy.html`
- Terms: `https://YOUR-USERNAME.github.io/app-legal-pages/shelfwise/terms.html`
- Support: `https://YOUR-USERNAME.github.io/app-legal-pages/shelfwise/support.html`

## 📱 Add to App Store Connect

1. Go to [App Store Connect](https://appstoreconnect.apple.com/)
2. Select your app
3. Go to **App Information**
4. Paste your Privacy Policy URL
5. Paste your Support URL (optional but recommended)

## 🔧 Customization Checklist

### Before Deploying SuperFusionGrid:
- [ ] Replace `[YOUR EMAIL HERE]` (appears in all 3 files)
- [ ] Replace `[YOUR JURISDICTION]` in terms.html
- [ ] Test all URLs work after deployment

### Before Deploying Shelfwise:
- [ ] Fill in all `[TODO:` sections in privacy.html
- [ ] Fill in all `[TODO:` sections in terms.html
- [ ] Fill in all `[TODO:` sections in support.html
- [ ] Replace email and jurisdiction placeholders
- [ ] Remove yellow TODO warning boxes
- [ ] Update "Last Updated" dates
- [ ] Test all URLs work after deployment

## 🎨 Customization Tips

The pages use clean, professional styling that matches iOS design language. If you want to customize:
- Colors are defined in the `<style>` section
- Primary color is `#007AFF` (iOS blue)
- Edit the HTML directly - no build process needed
- Commit and push changes to update live site

## 🌐 Want a Custom Domain?

Using your own domain (like `yourapps.com`) instead of GitHub Pages URLs?

**See the README.md** for complete custom domain setup instructions, including:
- How to register a domain
- DNS configuration (step-by-step)
- GitHub Pages + custom domain setup
- Netlify/Vercel alternatives
- Traditional web hosting options

You can start with GitHub Pages now and add a custom domain later - no code changes needed!

## ❓ Need Help?

Common issues:
- **404 error:** Wait 2-3 minutes after enabling Pages, check repository is Public
- **Changes not showing:** Clear browser cache or wait a few minutes
- **Wrong URL:** Make sure you're using YOUR-USERNAME, not the literal text

## 📝 Files Location

All files are in: `/Users/markbridge/Documents/app-legal-pages/`

You can edit them with any text editor or IDE.

---

**Ready to deploy SuperFusionGrid?** Just update the email/jurisdiction and push to GitHub!
