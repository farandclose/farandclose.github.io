# Far & Close

Plain HTML/CSS site for GitHub Pages; no build step (`.nojekyll` disables Jekyll).

## Preview
    python3 -m http.server 8000   # open http://localhost:8000

## Add a post
1. Copy `about/index.html` to `writing/<slug>/index.html`, change `<title>`, and replace the contents of `<div class="wrap">` inside `<main>` with your essay (`<h1>`, `<p>`, ...). Paths use `../../` for a two-level-deep page (fix `style.css` and nav hrefs accordingly).
2. Add a line under `<!-- POSTS: newest first -->` in BOTH `index.html` and `writing/index.html`:
   `<li><a href="/writing/<slug>/">Title</a><span class="meta">Oct 2026</span></li>`
3. Remove the "Coming soon" item once the Markwise post exists.
`_preview/` holds screenshots only; delete it before publishing if you like.
