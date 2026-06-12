# dannidanniwu.github.io

Personal academic website for Danni Wu, built with plain Jekyll (no theme dependency) on GitHub Pages.

## How to deploy

1. In your repo, **delete all old files** from the previous theme (everything from the RayeRen fork).
2. Copy all files from this folder into the repo root.
3. Commit and push to `main`. GitHub Pages builds it automatically — no Gemfile or Actions setup needed.

## How to write a blog post

Add a Markdown file to `_posts/` named `YYYY-MM-DD-short-title.md`:

```yaml
---
title: "My post title"
date: 2026-06-15
tags: [bayesian, R]
---

Your content in Markdown...
```

It appears on /blog/ automatically.

## Customizing

- **Photo**: add `images/profile.jpg`, then uncomment the `<img class="profile-photo">` line in `index.html`.
- **Links**: update Google Scholar / LinkedIn URLs in `_config.yml`.
- **CV**: replace `files/Danni_Wu_CV.pdf` whenever you update your CV.
- **Colors / fonts**: everything is in `assets/css/main.css` under `:root`.

## Preview locally (optional)

```bash
gem install jekyll bundler
jekyll serve
```
