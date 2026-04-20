# Bootstrap Beekeeping

**A first-year beekeeping blog and brand site**
Built by Josh M. · Centre, Alabama · © 2026 Bootstrap Beekeeping

Live at: [bootstrapbeekeeping.com](https://bootstrapbeekeeping.com)

---

## Overview

Bootstrap Beekeeping is the public-facing brand site for Bootstrap Beekeeping and Apiary HQ. It documents a first-year beekeeping journey in Cherokee County, Alabama, and serves as the marketing home for the Apiary HQ app.

- **Hosting:** Cloudflare Pages (auto-deploy from `main` branch)
- **Analytics:** Google Analytics 4 — `G-Y40NT4J5LG`
- **Email:** `admin@bootstrapbeekeeping.com` (Cloudflare routing → Gmail)
- **Subscribers:** Supabase project `hvunisdpkbejvenaesjf` — `subscribers` table
- **Search:** Google Search Console verified via Cloudflare DNS

---

## Site Structure

| File | Description |
|------|-------------|
| `index.html` | Homepage — auto-loads latest post from `posts/index.json` |
| `about.html` | Our Story — includes PawPaw/Sawyer legacy photo |
| `apiary.html` | Field Notes archive — auto-loads all posts from `posts/index.json` |
| `apiaryhq.html` | Apiary HQ product page |
| `honey.html` | Honey & Woodware (coming soon) |
| `privacy.html` | Privacy Policy |
| `sitemap.xml` | Submitted to Google Search Console |
| `posts/index.json` | Single source of truth for all posts |
| `posts/post-0XX.html` | Individual post files |

---

## Adding a New Post

1. Duplicate `posts/post-template.html` → rename to `posts/post-00X.html`
2. Fill in all placeholders in the new post file
3. Add a new entry to the **top** of `posts/index.json`
4. Add post image to `images/`
5. Push via GitHub Desktop

Both `index.html` (latest post) and `apiary.html` (full archive) update automatically from `index.json`. No manual HTML edits needed.

---

## Deployment Rules

- **Always push via GitHub Desktop only** — never use GitHub API directly (causes merge conflicts)
- Local repo path: `/Users/JoshM/Desktop/GitHub/bootstrap-beekeeping-site/`

---

## Design

- **Palette:** Navy `#1B2A4A` · Gold `#C8860A` · Cream `#F7F3E8` · Linen `#F0E8D5`
- **Fonts:** Playfair Display (headings) + Lora (body)
- **Pattern:** Honeycomb hex SVG overlay at 9% opacity
- **Nav:** Fixed top banner + hamburger drawer
