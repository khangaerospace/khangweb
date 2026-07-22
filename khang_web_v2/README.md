# Khang Nguyen — Portfolio v3

Modern dark aerospace-themed portfolio. 4 pages, pure HTML/CSS/JS, zero dependencies, zero build tools.

## Files
```
index.html    → Home (bio, skills, values, blog preview)
career.html   → Career timeline
blog.html     → Blog with category filter
contact.html  → Contact form
style.css     → Shared design system
README.md     → This file
```

---

## Deploy FREE on GitHub Pages

**1. Create the repo**
- Go to https://github.com/new
- Name it exactly: `khangaerospace.github.io`
- Set to **Public** → Create

**2. Upload files**
- On the repo page → "uploading an existing file"
- Upload all 5 files + your photo (`khangnguyenpic.jpg`)
- Commit to `main`

**3. Enable Pages**
- Repo Settings → Pages
- Source: Deploy from branch → `main` / `/ (root)`
- Save

**4. Done!**
Your site is live at: `https://khangaerospace.github.io`
(takes ~1 min to propagate)

**Custom domain (optional)**
- Buy a domain on Namecheap (~$10/yr)
- Settings → Pages → Custom domain → enter it
- Add a CNAME DNS record pointing to `khangaerospace.github.io`

---

## Set Up the Contact Form (Formspree)

1. Sign up free at https://formspree.io
2. Create a new form, copy the form ID from the endpoint (e.g. `xpznkqra`)
3. In `contact.html`, find:
   ```
   action="https://formspree.io/f/YOUR_FORM_ID"
   ```
   Replace `YOUR_FORM_ID` with your actual ID.
4. Push the change to GitHub — Pages redeploys automatically.

Free tier: **50 messages/month** — no backend needed.

---

## Add Your Photo

Put your photo in the root folder named `khangnguyenpic.jpg`.
Or change the `src` in `index.html` hero section to match your filename.

---

## Adding Career Entries

In `career.html`, find the comment:
```
<!-- ADD MORE: copy a .timeline-wrap block, update year, t-title, t-org, t-desc, t-tags, t-badge class -->
```
Copy any existing `.timeline-wrap` block and edit the content.

Badge classes: `badge-intern` | `badge-lead` | `badge-fellow` | `badge-vol`

---

## Adding Blog Posts

**Option A — Link externally** (what you're doing now)
Just add an `<a>` card to `#blog-grid` in `blog.html` pointing to the external URL.

**Option B — Write your own posts**
1. Create a `posts/` folder
2. Copy the HTML structure from any page, remove the hero/skills sections
3. Write your content in `<main>`
4. In `blog.html` set `href="posts/your-post-title.html"`

---

## Cost Summary

| | Cost |
|---|---|
| GitHub Pages hosting | **FREE** |
| Formspree contact form | **FREE** (50/mo) |
| Custom domain (optional) | ~$10–15/yr |
| **Total** | **$0** (or ~$10–15/yr with domain) |
