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

Push to `master` and it's live at `/projects/slug/`. A post dated in the future
won't publish until that date.

## Local preview

```bash
bundle install          # first time only
bundle exec jekyll serve # http://localhost:4000
```

## Adding or editing a project

`/projects/` and the home-page preview both render from the posts in `_posts/` — a
project is a case study, so `image:`, `stack:`, `links:` and `description:` in its
front matter feed the row. `height:` shortens the thumbnail box; omit it for 16:9.

Screenshots go in `assets/work/` as 1200px-wide JPEGs:

```bash
sips -Z 1200 --setProperty formatOptions 72 shot.png --out assets/work/name.jpg
```

## Layout

- `index.md` — splash first viewport, then the about copy. There is no `/about/` URL;
  the nav points at `/#about`, so that copy lives in exactly one place.
- `projects.md` — the one inner page. One layout, `_layouts/default.html`; case
  studies add `_layouts/post.html`.
- `_includes/` — `head.html`, `nav.html`, `socials.html` and `wordmark.html` (the
  letter-split name); `project-row.html` renders one row of the project list.
- `assets/css/main.css` — the whole design. No webfont, no accent colour: system sans,
  black on white, hairline rules. `.rows` is the one list shape reused by projects,
  experience, services and posts.

## Motion

All CSS, no JS, and every bit of it sits inside `@media (prefers-reduced-motion:
no-preference)` at the bottom of `main.css`:

- **Splash entrance** — face pops, then the name a letter at a time (`--i` on each
  letter drives the stagger), then the nav, then the socials.
- **Scroll morph** — on the home page only, one `scroll(root)` timeline fades the
  splash upward while the compact masthead drops in, so the page turns into an
  ordinary one as you scroll. `body.home` selects it.
- **Scroll reveals** — `animation-timeline: view()` on rows, section heads and the
  about block.

Both scroll effects are wrapped in `@supports`; without support the masthead is
simply always visible and nothing is hidden.
