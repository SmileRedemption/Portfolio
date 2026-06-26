# Denys Ismaylov — Unity Developer Portfolio

Portfolio site + CV. Live at: **https://[your-github-username].github.io/cv**

---

## How to enable GitHub Pages

1. Push this repo to GitHub (if not done yet):
   ```bash
   git add .
   git commit -m "Add portfolio site"
   git push
   ```

2. Go to your repo on GitHub → **Settings** → **Pages** (left sidebar)

3. Under **Source**, select:
   - Branch: `main`
   - Folder: `/docs`

4. Click **Save**

5. Wait ~1 minute. Your site will be live at:
   ```
   https://<your-github-username>.github.io/cv
   ```

---

## Before going live — update these in `docs/index.html`

| What | Where | Replace with |
|---|---|---|
| LinkedIn URL | `about__links` section + contact buttons | Your real LinkedIn URL |
| GitHub URL | `about__links` section | Your real GitHub URL |
| Google Play link | Street Dude card | Real Play Store URL |
| Phone number | Contact section | Check it's correct |
| CV download | Nav + Contact buttons | Points to your PDF |
| "Available for opportunities" badge | Hero | Change if not looking |

---

## Files

```
docs/
├── index.html          ← main page
├── styles.css          ← all styles
└── script.js           ← scroll animations, nav
Denys_Ismaylov_Unity_Developer.pdf   ← linked as CV download
RESUME_GUIDE.md         ← resume writing guide
README.md               ← this file
```

---

## Customization tips

- **Add a real screenshot/GIF for Street Dude** — drop an image into `docs/` and replace the
  placeholder icon in the Street Dude card with `<img src="street-dude.png" alt="Street Dude" />`
- **Add your photo** — replace the `.hero__badge` area or add an `<img>` in the about section
- **Update stats** — Hero section has 4 stats (years, downloads, LTV, platforms); edit in `index.html`
- **Add more projects** — copy a `.card` block and fill in your details
- **Custom domain** — buy `denysismaylov.dev` (~$10/yr), add a `CNAME` file in `docs/` with just
  your domain name, then configure DNS at your registrar
