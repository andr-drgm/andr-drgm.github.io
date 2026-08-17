# andrei-dragomir.com

Personal site and blog. Plain Jekyll — GitHub Pages builds it on push, no CI, no node.

## Writing a post

Create `_posts/YYYY-MM-DD-slug.md`:

```markdown
---
layout: post
title: "Post title"
description: One line for search results and link previews.
---

Body in markdown. Images go in `assets/posts/` and are referenced from root:

![alt text](/assets/posts/my-image.jpg)
```

Push to `master` and it's live at `/writing/slug/`. A post dated in the future
won't publish until that date.

## Local preview

```bash
bundle install          # first time only
bundle exec jekyll serve # http://localhost:4000
```

## Adding or editing a project

Project cards on `/` and `/work/` both render from **`_data/projects.yml`** — edit that one
file, not the pages. `featured: true` puts a project on the home page. `anchor:` must match a
heading id in the case-study post (`## Name {#anchor}`).

Card images live in `assets/work/` and are cropped to 16:9. Screenshots are 1200px wide JPEGs:

```bash
sips -Z 1200 --setProperty formatOptions 72 shot.png --out assets/work/name.jpg
```

## Layout

- `index.md`, `writing.md`, `work.md` — the three pages
- `_data/projects.yml` + `_includes/project-card.html` — project cards
- `_layouts/` — `default.html` (shell), `post.html` (post shell)
- `assets/css/main.css` — the whole design; colors and fonts are the `:root` tokens at the top.
  `--accent` is the only accent safe for body-size text; `--accent-warm` and `--ember` are for
  large type and decoration (they fail contrast at body size on this light background).
- Scroll reveals use native `animation-timeline: view()` — no JS. Browsers without support show
  content immediately, and `prefers-reduced-motion` disables all of it.
