# lcellentani.github.io

Source of my personal site, built with [Hugo](https://gohugo.io) and the
[PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme, and published to
GitHub Pages by GitHub Actions.

## Write a post

1. Create `content/posts/<short-name>/index.md` (put images in the same folder).
2. Write it in markdown. Start with this front matter:

   ```yaml
   ---
   title: "My title"
   date: 2026-11-01T09:00:00+01:00
   draft: false
   description: "One sentence for search results and link previews."
   tags: ["cpp"]
   ---
   ```

3. Commit and push to `master`. The site builds and publishes by itself.

Set `draft: true` to keep a post out of the build while you work on it.

## Preview locally (optional)

Install the extended Hugo (version 0.158 or newer), then run `hugo server -D` from
the repo root and open http://localhost:1313.

## How it is organized

- `content/` the posts.
- `hugo.toml` site title, menu, theme settings.
- `themes/PaperMod/` the theme, copied into the repo (MIT license). To update it,
  replace the folder with a newer copy.
- `static/` the old 2019 site as it was built by Hugo 0.56. It is kept so the old
  post URLs still work. Do not edit it.
- `.github/workflows/hugo.yaml` builds on every push, and deploys only from `master`.
