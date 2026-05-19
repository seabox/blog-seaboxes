# Seaboxes Blog

Personal blog of the Box family — primarily documenting Violet's cancer journey and life beyond it.

Live at [blog.seaboxes.com](https://blog.seaboxes.com)

## Architecture

- **Static site generator**: [Hugo](https://gohugo.io/) (Extended)
- **Theme**: [PaperMod](https://github.com/adityatelange/hugo-PaperMod) (git submodule)
- **Hosting**: GitHub Pages
- **Deployment**: GitHub Actions (`.github/workflows/hugo.yml`) — pushes to `master` trigger an automatic build and deploy

## Structure

```
content/posts/     # Blog posts (Markdown)
content/about.md   # About page
content/search.md  # Search page
content/archives.md# Archive page
static/assets/img/ # Images
layouts/partials/  # Custom partials (KaTeX + Mermaid support)
hugo.yaml          # Site configuration
```

## Local development

Requires [Hugo Extended](https://gohugo.io/installation/).

```bash
# Clone with submodules
git clone --recurse-submodules <repo-url>

# Serve locally (includes drafts)
hugo server -D
```

Site is available at http://localhost:1313/

## Writing a new post

Create a Markdown file in `content/posts/` named `YYYY-MM-DD-slug.md` with this front matter:

```yaml
---
title: Post Title
date: "YYYY-MM-DD HH:MM:00"
author: Craig
tags: [Tag1, Tag2]
cover:
  image: /assets/img/posts/your-image.jpg
---
```