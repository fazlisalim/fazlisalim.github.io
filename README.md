# fazlisalim.com — Website Guide

A personal academic website built with plain HTML, CSS, and JavaScript. No frameworks, no build tools — just files you can open and edit in any text editor.

---

## File Structure

```
fazlisalim/
├── index.html      ← Home page
├── about.html      ← About page
├── research.html   ← Research page
├── cv.html         ← CV page
├── writing.html    ← Writing & science communication
├── contact.html    ← Contact page
├── style.css       ← All styling (colors, fonts, layout)
├── script.js       ← Navigation toggle, scroll effects
├── photo.jpg       ← Your profile photo (replace this file)
├── cv.pdf          ← Your CV PDF (replace this file)
└── README.md       ← This file
```

---

## How to Edit Content

Open any `.html` file in a text editor (TextEdit on Mac, Notepad on Windows, or VS Code — recommended).

### Updating your bio text
Find the paragraph tags `<p>...</p>` and edit the text inside them.

### Updating links
Find `href="..."` and change the URL inside the quotes.
Example: `<a href="mailto:fazli.salim@bc.edu">` → change to your email address.

### Adding a new presentation
In `research.html`, find the `<div class="pres-list">` section and copy/paste a `<div class="pres-item">` block:
```html
<div class="pres-item">
  <span class="pres-year">2025</span>
  <div class="pres-detail">
    <p class="pres-conf">Conference Name</p>
    <p class="pres-loc">City · Month Year</p>
    <a href="LINK_TO_POSTER" target="_blank" class="pres-link">View poster →</a>
  </div>
</div>
```

### Adding a new writing piece
In `writing.html`, copy/paste a `<a class="writing-card">` block into the grid.

### Updating social links
Search for `https://scholar.google.com`, `https://twitter.com`, `https://linkedin.com` and replace with your actual profile URLs.

### Replacing your photo
Simply replace `photo.jpg` with your own photo file, keeping the same filename. The photo should ideally be portrait orientation, at least 440×560px.

### Updating your CV
Replace `cv.pdf` with your updated PDF file, keeping the same filename.

---

## Recommended Free Code Editor

**VS Code** (Visual Studio Code) — https://code.visualstudio.com/
- Free, works on Mac/Windows/Linux
- Install the **"Live Server"** extension to preview your site locally as you edit

---

## Deploying to GitHub Pages (Free Hosting)

### Step 1: Create a GitHub account
Go to https://github.com and sign up for free.

### Step 2: Create a new repository
1. Click the **+** button → "New repository"
2. Name it exactly: `yourusername.github.io` (replace with your GitHub username)
3. Set it to **Public**
4. Click "Create repository"

### Step 3: Upload your files
1. Click "uploading an existing file"
2. Drag all your site files into the upload area
3. Click "Commit changes"

Your site will be live at: `https://yourusername.github.io`

### Step 4: Connect your GoDaddy domain

**In GitHub:**
1. Go to your repository → Settings → Pages
2. Under "Custom domain", enter: `www.fazlisalim.com`
3. Click Save
4. Check "Enforce HTTPS"

**In GoDaddy:**
1. Log into GoDaddy → My Products → DNS
2. Delete any existing A records
3. Add these 4 A records (pointing to GitHub's IPs):
   - Type: A | Name: @ | Value: `185.199.108.153`
   - Type: A | Name: @ | Value: `185.199.109.153`
   - Type: A | Name: @ | Value: `185.199.110.153`
   - Type: A | Name: @ | Value: `185.199.111.153`
4. Add a CNAME record:
   - Type: CNAME | Name: www | Value: `yourusername.github.io`

DNS changes take up to 48 hours to fully propagate (usually much faster).

---

## Updating the Site in the Future

1. Edit the file(s) locally
2. Go to your GitHub repository
3. Click the file → pencil icon (edit) → paste your changes → "Commit changes"

Or use GitHub Desktop (https://desktop.github.com/) for a drag-and-drop workflow.

---

## Colors & Fonts (for reference)

The site uses two fonts loaded from Google Fonts:
- **Cormorant Garamond** — headings and display text
- **DM Sans** — body text and navigation

Main colors (defined in `style.css` as CSS variables):
- `--ink` — main dark text (`#1a1814`)
- `--forest` — accent green (`#2d6a4f`)
- `--parchment` — warm off-white background (`#faf8f4`)

To change the accent color, search for `--forest:` in `style.css` and change the hex value.

---

© 2025 Fazli Salim
