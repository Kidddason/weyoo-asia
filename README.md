# Weyoo Asia — Company Website

A static multi-page website for a laboratory / analytical equipment supplier.
Built with plain HTML + CSS + JavaScript — no build step, ready for GitHub Pages.

## Pages

| File | Page |
|------|------|
| `index.html` | Home |
| `about.html` | About Us |
| `products.html` | Products (full catalogue) |
| `brands.html` | Brands |
| `service.html` | Service & Support |
| `research-and-development.html` | Research & Development |
| `contact.html` | Contact (with enquiry form) |

Shared assets: `css/style.css`, `js/main.js`, `assets/` (logo + hero background).

## Run locally

From this folder:

```
python -m http.server 8000
```

Then open http://localhost:8000

## Customising it for your company

1. **Company name / contact details** — set to Weyoo Asia, `+86 173 3303 3393`,
   `jimtom3393@gmail.com`, and the Kuala Lumpur address across all pages.
2. **Logo** — the site loads `assets/logo.png`. Save your company logo image as
   `assets/logo.png` (a version with a transparent or white background looks best
   in the header).
3. **Brands** — `brands.html` shows real brand logo images from `assets/brands/`.
4. **Products** — full catalogue is in `products.html`.
5. **Contact form** — currently front-end only (shows a thank-you message). Connect it to a
   service like Formspree, or a backend, before going live.

## Publish to GitHub Pages

1. Create a new repository on GitHub.
2. In this folder:
   ```
   git init
   git add .
   git commit -m "Initial website"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   select `main` / `root`, save. Your site will be live at
   `https://<your-username>.github.io/<your-repo>/`.

## Custom domain

After buying a domain, in **Settings → Pages → Custom domain** enter your domain, then
add the DNS records your registrar requires (an `A` record set to GitHub Pages IPs, or a
`CNAME` record pointing to `<your-username>.github.io`). GitHub will issue an HTTPS
certificate automatically.
