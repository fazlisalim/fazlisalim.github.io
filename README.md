# fazlisalim.com 
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
