# Chaplaincy Pro — Holding Page

Single-page "Reconstruction in progress" placeholder for chaplaincy.pro while the new Buildor-based site is being built.

## Contents

- `index.html` — the page (self-contained except for Google Fonts CDN)
- `assets/` — required files:
  - `CP_LOGO-gradient.svg` (44px nav, desktop)
  - `Logo MIni.svg` (40px nav, mobile + favicon)
  - `Logo-Animation.webp` (not used by index.html, included for future variations)
  - `hero-video.mp4` (7.4 MB, desktop hero background)
  - `hero-video-mb.mp4` (7.7 MB, mobile hero background)
  - `hero-pattern.svg` (guilloche overlay)

**Total size:** ~16 MB

## Design

Matches the paper-and-brass aesthetic of the upcoming new site:
- Hero video bg + golden gradient + subtle guilloche pattern
- Glass-morphism content card (cream + soft gold + blur)
- Fraunces serif + Inter Tight sans + JetBrains Mono labels
- Cream `#F4F0E8` base, brass `#8A5A1F` accent

## Deployment

### Static hosting (Netlify, Vercel, Cloudflare Pages, GitHub Pages)
Just drop the entire `public-holding/` folder. The page is fully static.

### Drop into existing WordPress / cPanel
Replace `index.php` at site root with `index.html` from this folder, upload `assets/` next to it. WordPress will not be reachable until you remove the placeholder.

### Apache/Nginx subdomain
Point document root at this folder.

### Test locally
```
python -m http.server 8000
# or
npx serve .
```

Then open <http://localhost:8000/>.

## What is intentionally minimal

- No menu / no internal links (everything is "back soon")
- No newsletter signup (avoid email collection during transition — add later if desired)
- No social icons (focus is on the message)
- Only public contact (phone + email) and address
