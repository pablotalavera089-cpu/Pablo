# Pablo & Kaida — Duo Portfolio

A bright, modern duo portfolio with:
- full-screen admin overlay
- password gate
- editable site copy
- add/edit/delete/reorder for about, workshops, performances, gallery, reels, downloads, and schedule
- gallery slideshow and reels together
- contact page with a working email draft form
- localStorage persistence plus export/import JSON

## How to use

1. Upload the files to GitHub.
2. Turn on GitHub Pages.
3. Open the site and click **Login**.
4. Use the admin password from `main.js`.

## Admin password

Current password in this build:
`PabloKaida2026!`

The password is stored as a SHA-256 hash in `main.js`. To change it, generate a new SHA-256 hash and replace `ADMIN_PASSWORD_HASH`.

Example:
```bash
node -e "const crypto=require('crypto'); console.log(crypto.createHash('sha256').update('YOUR_PASSWORD').digest('hex'))"
```

## Important note

This admin dashboard is a front-end overlay for GitHub Pages. It is convenient for one-device editing and browser-saved content, but it is not the same as a server-side private CMS. For real multi-device protection, you would add Cloudflare Access or a backend.

## Contact form

The contact form opens an email draft, so it works on static hosting without extra services. If you later want direct sending, connect Formspree, Netlify Forms, or a custom backend.

## Google Drive downloads

Add your Drive links in the Media / Press section. Make sure the file sharing setting is **Anyone with the link can view**.
