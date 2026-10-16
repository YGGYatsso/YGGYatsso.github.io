# YGGYatsso.github.io

My personal blog, built with [Hugo](https://gohugo.io/) and the
[PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme, deployed to
GitHub Pages via GitHub Actions.

Live at: **https://yggyatsso.github.io/**

## Writing a post

1. Create a file `content/posts/YYYY-MM-DD-my-title.md`
2. Add front matter:

   ```markdown
   ---
   title: "My Title"
   date: 2026-10-16T10:00:00+05:30
   tags: ["deep-learning"]
   categories: ["ML"]
   summary: "One-line description shown on the home page."
   math: false        # set to true to enable LaTeX rendering
   draft: false
   ---
   ```

3. Write Markdown below the front matter. Commit and push to `main` — the
   site rebuilds automatically.

## Local preview

```bash
git clone --recurse-submodules https://github.com/YGGYatsso/YGGYatsso.github.io
cd YGGYatsso.github.io
hugo server -D
```

Open http://localhost:1313.

## Layout

```
content/
  posts/      # blog posts (Markdown)
  about.md    # About page
  archives.md # Archives page
  search.md   # Search page
layouts/
  partials/extend_head.html  # MathJax loader for `math: true` posts
hugo.toml     # site configuration
.github/workflows/hugo.yml   # deploy workflow
```
