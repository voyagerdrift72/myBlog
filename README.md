# Editorial Jekyll Blog

A modern Jekyll 4.x blog designed for GitHub Pages deployment with GitHub Actions.

## Technology

- Jekyll 4.4.x
- Ruby 3.3
- GitHub Actions deployment
- MathJax 3 for LaTeX
- Rouge for syntax highlighting
- Python fenced code blocks

## Run locally

Install Ruby 3.3, then run these commands from the project root:

```bash
bundle install
bundle exec jekyll serve
```

Open the local address printed by Jekyll.

## Deploy

1. Create a GitHub repository.
2. Upload the project contents.
3. In GitHub, open **Settings → Pages**.
4. Set **Source** to **GitHub Actions**.
5. Push to the `main` branch.

The workflow in `.github/workflows/pages.yml` builds and deploys the website.

## Writing posts

Create posts inside `_posts/` using:

```text
YYYY-MM-DD-your-title.md
```

Example:

```markdown
---
layout: post
title: "My New Idea"
subtitle: "An optional subtitle."
---

Your text.

$$
E = mc^2
$$

```python
print("Hello")
```
```
