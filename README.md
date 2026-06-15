# Ryan Bourke — Audio Engineer Website

This is the source code for Ryan Bourke's personal website, built with Jekyll and hosted on GitHub Pages.

---

## Quick Reference: How to Edit the Site

Everything is in plain text files (Markdown). You can edit directly on GitHub by navigating to a file and clicking the pencil icon ✏️, or edit locally and push.

### Banner Text
**File:** `_includes/marquee.html`

Change the text inside the `<span>` tags. Keep the `&nbsp;` at the end of each span.

### Homepage Album Grid
The homepage automatically shows every item in the `_portfolio/` folder as a square image.

**To add a new album:**
1. Copy an existing file in `_portfolio/` (e.g., `album-01.md`).
2. Rename it (e.g., `my-new-project.md`).
3. Edit the top section (YAML front matter):
   - `title:` — Artist — Album Title
   - `excerpt:` — Your role (e.g., "Mixing, Mastering")
   - `header.teaser:` — Filename of the cover image (must be in `images/`)
4. Add a description in the body of the file (below the `---`).
5. Upload the cover image to the `images/` folder.

**To remove an album:** Delete its `.md` file from `_portfolio/`.

### About Page
**File:** `_pages/about.md`

- Edit the bio text directly.
- Replace the photo paths in the `<img>` tags (upload new photos to `images/`).
- Edit the gear table by changing the text inside the `<td>` tags.

### Credits / Discography
**File:** `_pages/credits.md`

Add new entries by copying an existing `<li>...</li>` line and editing it.
Add new years by copying a full year block (`## Year` through `</ul>`).

### Services
**File:** `_pages/services.md`

Edit the text inside each service card. Add new cards by copying a full `<div class="service-card">...</div>` block.

### Contact
**File:** `_pages/contact.md`

Change the email address in both the `mailto:` link and the displayed text.

### Site Settings (Name, Description, Social Links)
**File:** `_config.yml`

Edit the top section. After changing this file, the site may take a minute to rebuild.

### Navigation Menu
**File:** `_data/navigation.yml`

Add, remove, or reorder menu items here.

---

## Preview Locally

If you want to see changes before pushing to GitHub:

```bash
bundle install
bundle exec jekyll serve --livereload
```

Then open http://localhost:4000 in your browser.

---

## Folder Structure

| Folder | Purpose |
|--------|---------|
| `_pages/` | Main pages: About, Credits, Services, Contact |
| `_portfolio/` | Album/project entries that appear on the homepage grid |
| `images/` | Photos, album covers, and other images |
| `assets/css/custom.css` | Custom styles (fonts, colors, layout) |
| `_includes/marquee.html` | The scrolling banner at the top |
| `_config.yml` | Site-wide settings |
| `_data/navigation.yml` | Top menu links |

---

## Need Help?

If something breaks, the [Academic Pages guide](https://academicpages.github.io/markdown/) has general Jekyll/Markdown help. Or reach out to Nicola 😀
