# Shishir Sharma — Portfolio

A single-page portfolio site (dark, terminal-inspired theme), built with plain HTML/CSS/JS — no build step, so it works directly with GitHub Pages.

## Before you publish

Open `index.html` and search for `[Add` — three experience entries (Thomson Reuters, Netflix, Tata Consultancy Services) have placeholder titles/dates since I didn't have your exact role titles and employment dates for those. Fill those in (and delete the `<div class="edit-note">` lines) before going live. Everything else (Walmart Mexico role, achievements, skills, contact links) is filled in from what you've shared.

## Deploy to GitHub Pages (free hosting)

I don't have push access to your GitHub account from here, so getting this live still needs one action from you — but it can be done entirely in the browser, no git or terminal required:

### Easiest: upload via GitHub's website (no git needed)

1. Go to **https://github.com/new**, name the repo `shis2405.github.io` (must match this exactly — it makes the site live at your root domain), leave it public, click **Create repository**.
2. On the new repo page, click **uploading an existing file** (or "Add file → Upload files").
3. Drag in `index.html` and `README.md` from this folder, then click **Commit changes**.
4. Go to **Settings → Pages** in that repo → under "Build and deployment" set **Source: Deploy from a branch**, branch **main**, folder **/(root)** → **Save**.
5. Within a minute or two, your site is live at **https://shis2405.github.io** — permanently, for free, with no further steps needed. Any time you want to update it, just re-upload the changed file the same way.

### Alternative: git command line

If you'd rather use git, you have two options — pick whichever repo name you want:

### Option A: `shis2405.github.io` (site lives at the root domain)

```bash
cd shishir-portfolio
git init
git add index.html README.md
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/shis2405/shis2405.github.io.git
git push -u origin main
```

Then go to your repo → **Settings → Pages** → under "Build and deployment", set **Source: Deploy from a branch**, branch **main**, folder **/(root)** → Save.

Your site will be live at:
**https://shis2405.github.io**

(First create the empty repo at github.com/new named exactly `shis2405.github.io` before running the commands above.)

### Option B: Any repo name (site lives at a sub-path)

```bash
cd shishir-portfolio
git init
git add index.html README.md
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/shis2405/portfolio.git
git push -u origin main
```

Same Settings → Pages steps as above. Your site will be live at:
**https://shis2405.github.io/portfolio**

(Create the empty repo at github.com/new named `portfolio`, or whatever name you like, first.)

## Updating the site later

Edit `index.html`, then:

```bash
git add index.html
git commit -m "Update content"
git push
```

GitHub Pages redeploys automatically within a minute or two.
