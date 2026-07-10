# Internship Reflection Blog

Plain HTML/CSS static blog, built to deploy on GitHub Pages.

## Deploy to GitHub Pages

1. Create a new GitHub repo (public), e.g. `internship-blog`.
2. Push everything in this folder to the repo root.
3. Go to **Settings > Pages** in the repo.
4. Under "Build and deployment," set Source to **Deploy from a branch**,
   branch `main`, folder `/ (root)`. Save.
5. Your site goes live at `https://YOUR-USERNAME.github.io/REPO-NAME/`
   (takes ~1 minute after the first push).

## Turn on comments (Giscus)

Giscus uses your repo's GitHub Discussions as the comment backend — free,
no server needed, works great with GitHub Pages.

1. In your repo: **Settings > General > Features > check "Discussions."**
2. Go to https://giscus.app and enter your repo name.
3. Pick (or create) a Discussion category to post comments into.
4. Giscus generates a `<script>` snippet with your real `data-repo-id`
   and `data-category-id` filled in.
5. Copy that snippet into every post file, replacing the placeholder
   `<script>` block near the bottom (look for `data-repo="YOUR-GITHUB..."`).

Do this once and comments work on every post that has the snippet.

## Adding a new weekly post

1. Copy `posts/_template.html`, rename it something like
   `posts/week-02-reflection.html`.
2. Fill in the bracketed/placeholder sections.
3. Paste in your real giscus snippet (same one from setup above).
4. Add a new `<a class="ticket">` block to the top of `index.html`
   (copy the Week 1 block, edit the ticket number/title/summary/link).
5. Commit and push — GitHub Pages updates automatically.

## File structure

```
index.html          → homepage / entry list
about.html           → about page
assets/style.css     → all styling
posts/
  week-01-reflection.html   → first entry (edit the placeholder sections)
  _template.html            → copy this for every new week
```
