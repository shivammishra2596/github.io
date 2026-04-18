# Shivam Mishra — Personal Website

Personal brand site built with static HTML/CSS/JS. Deployed via GitHub Pages.

---

## File Structure

```
/
├── index.html          ← Your entire website (one file)
├── README.md           ← This file
└── images/
    ├── shivam.jpg      ← Your headshot (About section)
    ├── kerala-1.jpg    ← Kerala backwaters photo
    ├── kerala-2.jpg    ← Munnar tea gardens photo
    └── kerala-3.jpg    ← Varkala cliff/sunset photo
```

---

## Adding Your Photos

1. Create a folder called `images/` in the same directory as `index.html`
2. Add your photos with exactly these filenames (or update the `src=""` paths in index.html):
   - `images/shivam.jpg` — your headshot
   - `images/kerala-1.jpg` — backwaters / houseboat
   - `images/kerala-2.jpg` — Munnar tea gardens
   - `images/kerala-3.jpg` — Varkala sunset
3. Phone photos are fine. Landscape photos work best for Kerala. Portrait/square for your headshot.

---

## Making the Contact Form Work

1. Go to [https://formspree.io](https://formspree.io) and create a free account
2. Create a new form → copy your Form ID (e.g. `abcd1234`)
3. In `index.html`, find this line:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
4. Replace `YOUR_FORM_ID` with your actual ID:
   ```html
   <form action="https://formspree.io/f/abcd1234" method="POST">
   ```
5. Done — form submissions will arrive in your email.

---

## Deploying to GitHub Pages (Step-by-Step)

### Step 1 — Create your GitHub repo
- Go to [github.com](https://github.com) → New repository
- Name it: `shivammishra2596.github.io`
  *(Your GitHub username followed by `.github.io` — this gives you the root URL)*
- Set it to **Public**
- Click **Create repository**

### Step 2 — Upload your files
**Option A — Via GitHub website (easiest):**
1. Open your new repo
2. Click **Add file → Upload files**
3. Drag and drop `index.html`, `README.md`, and your `images/` folder
4. Click **Commit changes**

**Option B — Via Git CLI:**
```bash
git init
git add .
git commit -m "Initial site launch"
git branch -M main
git remote add origin https://github.com/shivammishra2596/shivammishra2596.github.io.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. Go to your repo → **Settings** → **Pages** (left sidebar)
2. Under **Source**, select `Deploy from a branch`
3. Choose branch: `main`, folder: `/ (root)`
4. Click **Save**

### Step 4 — Your site is live!
After 1–2 minutes, visit:
```
https://shivammishra2596.github.io
```

---

## Customising Content

All content is in `index.html`. Search for these comments to find key sections:

| What to change | Search for |
|---|---|
| Hero quote | `hero-philosophy` |
| About bio | `about-body` |
| Stats (numbers) | `stat-number` |
| Work experience | `timeline-item` |
| Kerala story | `story-text` |
| Contact email | `shivammishra2517281` |
| Social links | `contact-links` |

---

## Optional: Custom Domain (e.g. shivammishra.com)

1. Buy a domain from Namecheap, GoDaddy, or Google Domains (~₹800–1200/year)
2. In your domain's DNS settings, add a `CNAME` record:
   - Name: `www`
   - Value: `shivammishra2596.github.io`
3. In GitHub Pages settings → add your custom domain
4. Check "Enforce HTTPS"

---

*Built with ♥ — one file, zero frameworks, full character.*
