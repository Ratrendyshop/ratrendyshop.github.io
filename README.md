# Ratrendyshop

A clean, modern affiliate site for trending **home office productivity gadgets**, curated by Ratrendyshop and promoted on Pinterest & Instagram ([@Ratrendyshop](https://pinterest.com/Ratrendyshop)).

🔗 **Live site:** https://ratrendyshop.github.io

---

## What this is

A single-page, fully responsive website built as one self-contained `index.html` file — no build step, no dependencies, no framework. Just upload and it works.

**Sections**
- Hero with a Pinterest-style pinboard
- Trending gadget grid (masonry layout + category filters)
- Editor's Picks product spotlights
- Email capture for the free *Home Office Gadget Guide*
- Pinterest & Instagram follow cards
- FTC affiliate disclosure + footer

---

## Customizing it

Everything lives in `index.html`. Two things to set before promoting the site:

### 1. Affiliate links
Every "Shop on AliExpress" button uses a placeholder. Find and replace this across the file:

```
PASTE_AFFILIATE_LINK   →   your real AliExpress affiliate URL
```

Links already include `rel="nofollow sponsored"`, which is the correct setting for affiliate links.

### 2. Product photos
Each card shows a clean SVG placeholder. To use a real photo, replace a placeholder block:

```html
<div class="ph" data-art="stand"></div>
```

with an image:

```html
<img class="pin-photo" src="images/your-photo.jpg" alt="AeroRise Laptop Stand">
```

Vertical (2:3) images perform best on Pinterest.

### 3. Email signups (optional)
The signup form shows a success message by default. To actually collect emails, connect it to Mailchimp, ConvertKit, or Beehiiv — look for the `// TODO` marker in the `<script>` section.

---

## Updating the live site

1. Edit `index.html` (or upload a new version) in this repo.
2. Commit the change.
3. The live site refreshes within 1–2 minutes. Hard-refresh your browser (Ctrl/Cmd + Shift + R) to clear the cache.

---

## Hosting

Deployed with **GitHub Pages** (Settings ▸ Pages ▸ Deploy from branch ▸ `main` / root).

---

© Ratrendyshop. As an AliExpress affiliate, we earn from qualifying purchases.
