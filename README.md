# HORys — Legal (Privacy & Terms)

Static legal page for HORys Telegram bot, hosted on GitHub Pages.

- **Privacy Policy** — PDPA-compliant (Thailand B.E. 2562 / 2019)
- **Terms of Service** — covers AI-generated content disclaimer
- **Bilingual** — EN / TH toggle (Thai default)
- **Public** — no authentication required

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `horys-legal`), public
2. From this folder, push to GitHub:

   ```bash
   cd "/Users/taron/Desktop/Horoscope Projects /horys-legal"
   git init
   git add .
   git commit -m "Initial: HORys legal page (Privacy + Terms, EN/TH)"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/horys-legal.git
   git push -u origin main
   ```

3. Enable Pages: **Repo → Settings → Pages → Source = `main` branch, root (`/`) → Save**

4. Wait ~1 minute, then your site is live at:

   ```
   https://YOUR_USERNAME.github.io/horys-legal/
   ```

## Updating content

Edit `index.html` (everything is in one file — content, layout, JS).
After commit + push, GitHub Pages rebuilds in ~1 minute.

## Custom domain (optional)

1. Add `CNAME` file containing your domain (e.g. `legal.horys.app`)
2. In your domain DNS, add CNAME record pointing to `YOUR_USERNAME.github.io`
3. **Repo → Settings → Pages → Custom domain** = your domain → Save

## Files

```
horys-legal/
├── index.html              — main page (Privacy + Terms with EN/TH toggle)
├── static/
│   ├── horys.css           — design tokens (colors, spacing, fonts)
│   ├── horys-dashboard.css — shared component styles
│   └── horys-mark.svg      — HORys logo
└── README.md
```

## Versioning

Current document version: **1.0**
Effective date: **8 May 2026**

When updating Privacy or Terms content, bump the version + effective date in `index.html`:

```html
<span><span class="key">Version</span><span id="docVersion">1.0</span></span>
...
<span><span class="key">Effective</span><span id="effectiveDate">8 May 2026</span></span>
```

## Contact

Operator email is set in two places (Section 15 of Privacy + Section 18 of Terms):
- `taronx.ai@gmail.com`
