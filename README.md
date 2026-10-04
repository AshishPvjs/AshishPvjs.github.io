# ashishpvjs.github.io

Personal portfolio, projects, and blog — built with Jekyll and hosted on GitHub Pages.

## Structure

- `index.md` — home page (hero + latest posts)
- `about.md` — about page
- `projects.md` — project cards (edit these with real projects)
- `blog.md` — blog listing page
- `_posts/` — blog posts, one file per post, named `YYYY-MM-DD-title.md`
- `assets/css/style.scss` — custom styles on top of the `minima` theme
- `_config.yml` — site settings and navigation

## Writing a new blog post

Add a file to `_posts/` named `YYYY-MM-DD-your-title.md`:

```markdown
---
layout: post
title: "Your Title"
date: 2026-01-01 00:00:00 +0000
categories: misc
---

Your content here, in Markdown.
```

## Local preview (optional)

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000

## Deploying

Just push to the `main` branch — GitHub Pages builds and deploys automatically
(enable it once under repo Settings → Pages → Source → `main` branch).
