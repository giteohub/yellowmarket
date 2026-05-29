# YellowMarket — Deploy Instructions

## Sites buildés

### YellowMarket Agency Site
- **File:** `/home/teo/yellowmarket/index.html`
- **Pages:** Home, Services (3 pricing packages), About, Contact
- **Design:** Navy + gold, mobile-first, professional

### Demo Sites (pour prospection)
| Demo | File | Industry |
|------|------|----------|
| Central Valley Plumbing | `/home/teo/yellowmarket/demos/plumber/index.html` | Plumber |
| Bella Vita Ristorante | `/home/teo/yellowmarket/demos/restaurant/index.html` | Restaurant |
| BrightSmile Dental Care | `/home/teo/yellowmarket/demos/dentist/index.html` | Dentist |

---

## Deploy Options

### Option A — Hostinger Horizons (recommandé)
1. Connect to [horizons.hostinger.com](https://horizons.hostinger.com)
2. Create new project → "Import HTML"
3. Copy-paste the HTML content of each site
4. Publish to subdomain (yellowmarket.hostingerapp.com)
5. Connect custom domain (yellowmarket.co) → Settings → Domain

### Option B — GitHub Pages (free, no hosting cost)
```bash
cd /home/teo/yellowmarket
git init
git add .
git commit -m "Initial deploy"
gh repo create yellowmarket --public --push
# Enable GitHub Pages in repo Settings → Pages → deploy from main branch
# Site will be at: https://<username>.github.io/yellowmarket/
```

### Option C — Direct via Hostinger File Manager
1. Login to Hostinger → File Manager
2. Upload `index.html` to `public_html/` for main site
3. Create subdirectories for demos: `demos/plumber/`, `demos/restaurant/`, `demos/dentist/`
4. Upload each HTML file to its directory

---

## SEO Quick Check (avant mise en ligne)
- [ ] Meta titles personnalisés par page
- [ ] Meta descriptions
- [ ] Open Graph tags (share preview)
- [ ] Alt text on images (quand vraies photos ajoutées)
- [ ] Google Search Console soumis
- [ ] Canonical URL correct
- [ ] mobile-first responsive (déjà fait ✅)
