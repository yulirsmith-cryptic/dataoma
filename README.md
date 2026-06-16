# Dataoma

Marketing site for **Dataoma** — _Complex data into decisions._

Dataoma is an AI firm that automates reporting, makes data usable, and proves impact for organizations in any sector.

## What this is

A single-page, dependency-free static site (`index.html`) plus favicon assets and a logo. No build step, no framework. Fonts load from Google Fonts; everything else is self-contained.

## Before you launch: two quick edits

1. **Connect the contact form** (2 minutes)
   - Create a free account at [formspree.io](https://formspree.io) and make a new form.
   - Copy your form endpoint (looks like `https://formspree.io/f/abcdwxyz`).
   - In `index.html`, find `action="https://formspree.io/f/YOUR_FORM_ID"` and replace `YOUR_FORM_ID` with your real ID.
   - Until you do this, the form shows a friendly "not connected yet" message instead of failing silently.

2. **Set your contact email**
   - Replace `hello@dataoma.com` (appears in the footer and as the form's fallback) with your real address.

## Deploy to GitHub Pages

1. Push all files to a new repo's `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial Dataoma site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/dataoma-site.git
   git push -u origin main
   ```
2. Repo **Settings → Pages → Build and deployment**.
3. **Source**: *Deploy from a branch*; **Branch**: `main` / `root`; save.
4. Live at `https://<your-username>.github.io/dataoma-site/` in a minute or two.

### Custom domain (optional)
- Add your domain in **Settings → Pages → Custom domain** (e.g. `dataoma.com`).
- Point DNS: a `CNAME` record to `<your-username>.github.io`, or `A` records to GitHub Pages IPs.

## Editing

- All copy, colors, and type live in `index.html`. Colors are CSS variables at the top of the `<style>` block (`--ink`, `--paper`, `--signal`, etc.).

## Files

| File | Purpose |
|------|---------|
| `index.html` | The entire site |
| `logo.svg` | Standalone Dataoma wordmark lockup (dark version, for light backgrounds) |
| `favicon.ico` | Browser tab icon (16 + 32px) |
| `favicon-16.png`, `favicon-32.png` | PNG favicons |
| `apple-touch-icon.png` | iOS home-screen icon (180px) |
| `android-chrome-192x192.png`, `android-chrome-512x512.png` | Android / PWA icons |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |
| `README.md` | This file |

## The logo

The logo is the **Dataoma wordmark** set in Space Grotesk, with a teal macron over "oma" (cueing the long "oh" sound) and a small stack of bars trailing off the end of the word, descending into a teal signal node — the moment scattered data resolves into a decision. The favicon and app icons use a condensed version of that bar-and-node mark so the identity reads even at 16px.
