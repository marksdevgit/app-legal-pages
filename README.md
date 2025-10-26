# App Legal Pages

This repository contains Privacy Policies, Terms of Service, and Support pages for iOS apps, required for App Store submission.

## 📁 Structure

```
app-legal-pages/
├── index.html                    # Landing page linking to all apps
├── superfusiongrid/
│   ├── privacy.html             # Privacy Policy (Complete ✅)
│   ├── terms.html               # Terms of Service (Complete ✅)
│   └── support.html             # Support Page (Complete ✅)
├── shelfwise/
│   ├── privacy.html             # Privacy Policy (Template - TODO)
│   ├── terms.html               # Terms of Service (Template - TODO)
│   └── support.html             # Support Page (Template - TODO)
└── README.md                     # This file
```

## 🚀 Deployment to GitHub Pages

### Option 1: New Repository

1. **Create a new GitHub repository:**
   ```bash
   # Create repo on GitHub first, then:
   cd /Users/markbridge/Documents/app-legal-pages
   git init
   git add .
   git commit -m "Initial commit: Add legal pages for SuperFusionGrid and Shelfwise"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/app-legal-pages.git
   git push -u origin main
   ```

2. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click **Settings** → **Pages**
   - Under "Source", select **main** branch
   - Click **Save**
   - Your site will be live at: `https://YOUR-USERNAME.github.io/app-legal-pages/`

### Option 2: Use Existing Repository

If you already have a GitHub repository for your apps:

1. Copy these files into your existing repo
2. Enable GitHub Pages in Settings → Pages
3. Access via: `https://YOUR-USERNAME.github.io/REPO-NAME/`

## 🔗 URLs to Use in App Store Connect

Once deployed, use these URLs in your App Store Connect submission:

### SuperFusionGrid
- **Privacy Policy URL:** `https://YOUR-USERNAME.github.io/app-legal-pages/superfusiongrid/privacy.html`
- **Terms of Service URL:** `https://YOUR-USERNAME.github.io/app-legal-pages/superfusiongrid/terms.html`
- **Support URL:** `https://YOUR-USERNAME.github.io/app-legal-pages/superfusiongrid/support.html`

### Shelfwise
- **Privacy Policy URL:** `https://YOUR-USERNAME.github.io/app-legal-pages/shelfwise/privacy.html`
- **Terms of Service URL:** `https://YOUR-USERNAME.github.io/app-legal-pages/shelfwise/terms.html`
- **Support URL:** `https://YOUR-USERNAME.github.io/app-legal-pages/shelfwise/support.html`

## ✏️ Customization

### SuperFusionGrid
✅ **Complete** - Ready to deploy!

**Before deploying, update:**
- `[YOUR EMAIL HERE]` in all three files
- `[YOUR JURISDICTION]` in terms.html (e.g., "the United Kingdom" or "California, USA")

### Shelfwise
⚠️ **Needs Customization** - Template files with TODO markers

**To complete:**
1. Open each Shelfwise HTML file
2. Search for `[TODO:` markers
3. Fill in app-specific details:
   - What data does Shelfwise collect?
   - Does it use camera/barcode scanning?
   - Does it sync with iCloud or other services?
   - What third-party APIs does it use?
   - What are the key features?
4. Replace `[YOUR EMAIL HERE]` and other placeholders
5. Remove TODO warning boxes once complete

## 📝 Important Notes

1. **Privacy Policy is REQUIRED** by Apple for App Store submission
2. **Support URL is highly recommended** for user assistance
3. **Terms of Service is optional** but recommended for legal protection
4. These pages must be **publicly accessible** (not behind login)
5. Update the "Last Updated" dates when you make changes

## 🔄 Updating Pages

When you need to update a page:

```bash
cd /Users/markbridge/Documents/app-legal-pages
# Make your edits
git add .
git commit -m "Update privacy policy for [feature]"
git push
```

Changes will be live on GitHub Pages within a few minutes.

## 🌐 Custom Domain Setup

Want to use your own domain instead of GitHub Pages URLs? Easy!

### Benefits of Custom Domain
- **Professional appearance:** `yourdomain.com/superfusiongrid/privacy.html`
- **Brand consistency:** All legal pages under your domain
- **Portability:** Move hosting providers without changing URLs
- **Trust:** Custom domains look more professional in App Store Connect

### Option 1: GitHub Pages + Custom Domain (Recommended)

**Step 1: Deploy to GitHub Pages First**
Follow the deployment instructions above to get your site live on GitHub Pages.

**Step 2: Register a Domain**
Purchase a domain from any registrar:
- [Namecheap](https://www.namecheap.com/) - Budget-friendly
- [Google Domains](https://domains.google/) - Easy management
- [Cloudflare](https://www.cloudflare.com/products/registrar/) - At-cost pricing
- [Hover](https://www.hover.com/) - Clean interface

Popular extensions for apps:
- `.dev` - Developer/tech focus
- `.app` - App-specific
- `.io` - Tech-friendly
- `.com` - Classic professional

**Step 3: Configure Custom Domain in GitHub**
1. Go to your repository on GitHub
2. Navigate to **Settings** → **Pages**
3. Under "Custom domain", enter your domain (e.g., `yourapps.com`)
4. Click **Save**
5. Check **Enforce HTTPS** (wait a few minutes for SSL certificate)

**Step 4: Update DNS Records at Your Domain Registrar**

Choose ONE of these methods:

**Method A: CNAME Record (Subdomain - Recommended)**
If using `apps.yourdomain.com` or `www.yourdomain.com`:
```
Type:  CNAME
Name:  apps (or www)
Value: YOUR-USERNAME.github.io
TTL:   3600
```

**Method B: A Records (Apex Domain)**
If using `yourdomain.com` (no subdomain):
```
Type:  A
Name:  @ (or leave blank)
Value: 185.199.108.153
TTL:   3600

Add three more A records with these IPs:
185.199.109.153
185.199.110.153
185.199.111.153
```

Also add a `www` CNAME:
```
Type:  CNAME
Name:  www
Value: YOUR-USERNAME.github.io
TTL:   3600
```

**Step 5: Wait for DNS Propagation**
- Can take 5 minutes to 48 hours (usually under 1 hour)
- Check status: [whatsmydns.net](https://www.whatsmydns.net/)

**Step 6: Update Your URLs**
Your pages will now be accessible at:
```
https://yourdomain.com/superfusiongrid/privacy.html
https://yourdomain.com/shelfwise/privacy.html
```

Update these URLs in App Store Connect!

### Option 2: Netlify + Custom Domain (Easier DNS)

**Step 1: Deploy to Netlify**
1. Create account at [netlify.com](https://www.netlify.com/)
2. Drag and drop `/app-legal-pages/` folder
3. Get instant URL: `https://random-name.netlify.app/`

**Step 2: Add Custom Domain**
1. Click **Domain settings** in Netlify dashboard
2. Click **Add custom domain**
3. Enter your domain name
4. Follow Netlify's DNS instructions (they show exactly what to do)

**Benefits:**
- Netlify provides step-by-step DNS guidance
- Faster deployment than GitHub Pages
- Better CDN (faster worldwide)
- Automatic SSL
- Deploy previews for changes

### Option 3: Vercel + Custom Domain

1. Import folder at [vercel.com](https://vercel.com/)
2. Add domain in project settings
3. Follow DNS instructions
4. Same benefits as Netlify

### Option 4: Traditional Web Hosting

If you have existing web hosting (cPanel, shared hosting, VPS):

1. **Upload via FTP/SFTP:**
   - Connect to your hosting
   - Upload all files to `/public_html/` or web root
   - Or create subdirectory: `/public_html/apps/`

2. **Your URLs will be:**
   ```
   https://yourdomain.com/superfusiongrid/privacy.html
   https://yourdomain.com/apps/superfusiongrid/privacy.html (if in subdirectory)
   ```

3. **Ensure HTTPS:**
   - Most hosts offer free SSL (Let's Encrypt)
   - Enable in cPanel → SSL/TLS

## 🛠️ Alternative Free Hosting (No Custom Domain)

If you don't want to buy a domain yet:

### Netlify (Free)
1. Drag and drop this folder at [netlify.com](https://www.netlify.com/)
2. Get instant URL: `https://your-app-name.netlify.app/`

### Vercel (Free)
1. Import this folder at [vercel.com](https://vercel.com/)
2. Get instant URL: `https://your-app-name.vercel.app/`

Both provide free `.netlify.app` or `.vercel.app` subdomains that work fine for App Store submission.

## 📧 Contact Information

Before deploying, make sure to replace all instances of:
- `[YOUR EMAIL HERE]` - Your support email address
- `[YOUR JURISDICTION]` - Your legal jurisdiction for Terms of Service

## 📱 App Store Submission Checklist

- [ ] Deploy legal pages to GitHub Pages (or alternative)
- [ ] Test all URLs are publicly accessible
- [ ] Add Privacy Policy URL to App Store Connect
- [ ] Add Support URL to App Store Connect
- [ ] Add Terms of Service URL (optional)
- [ ] Complete Shelfwise template before submitting that app

## 🔄 Migration Between Hosting Providers

**The beauty of static HTML:** These files work anywhere! No code changes needed.

If you start with GitHub Pages and later want to move:
1. Download/clone your repository
2. Upload files to new hosting
3. Update URLs in App Store Connect
4. That's it!

You can easily migrate between:
- GitHub Pages ↔️ Netlify ↔️ Vercel ↔️ Your own hosting

No vendor lock-in, complete portability.

## 📄 License

These legal documents are templates for your personal apps. Customize them as needed for your specific use case.

---

**Created:** October 22, 2025
**Last Updated:** October 22, 2025
