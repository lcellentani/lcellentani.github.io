# Task: preview and publish the new Hugo site

You are working inside my local checkout of `lcellentani.github.io`. A new Hugo site was prepared on the remote branch `hugo-setup`. Your job is to help me preview it, fix anything that looks wrong, and then publish it. Do the steps in order, and stop where a step says "ask me".

## Rules

- Do not push to `master`, merge, or force-push unless I say so in this session.
- Do not delete files in `static/`. It holds the old 2019 site, kept so old URLs still work.
- You cannot change GitHub Pages settings. When that step comes, tell me exactly what to click.
- Keep changes small. Fix what is broken, and don't redesign anything.

## Background

- The branch `hugo-setup` has one commit with: `hugo.toml`, the PaperMod theme in `themes/PaperMod/`, the first post in `content/posts/what-eight-repos-taught-me/`, the old site moved into `static/`, a workflow in `.github/workflows/hugo.yaml`, and a README.
- The workflow builds on every push and deploys only from `master`.
- PaperMod needs the extended Hugo, version 0.158 or newer.
- The default branch is `master`.

## Steps

1. **Get the branch.** Run `git fetch origin` and check out `hugo-setup`. If I have uncommitted changes, stop and ask me.
2. **Check Hugo.** Run `hugo version`. If it is missing or older than 0.158, tell me how to install the extended version (Windows: `winget install Hugo.Hugo.Extended`; macOS: `brew install hugo`) and wait.
3. **Build.** Run `hugo --gc --minify` and report any warnings or errors. Fix problems in config or content only, and show me each change before committing.
4. **Preview.** Start `hugo server -D` and tell me to open http://localhost:1313. Ask me to confirm each of these:
   - The home page shows my name and the intro line, and the menu has Posts, Archive 2019 and Tags.
   - The post opens, the timeline chart is visible, and the repo links work.
   - `/post/cpp_rvo/` (an old post) still opens, and the "Archive 2019" link lists the old posts.
   - Light and dark themes both look fine.
5. **Fix and commit.** Commit any fixes on `hugo-setup` with a clear message, and ask me before pushing.
6. **Publish (ask me first).** Tell me to do these two things within a minute or two of each other:
   - On GitHub: repo Settings, then Pages, then set the source to "GitHub Actions".
   - Merge `hugo-setup` into `master` (open a pull request, or merge locally if I say so).
7. **Verify.** After the deploy finishes (the Actions tab shows "Build and deploy site" green), open https://lcellentani.github.io/ and check the home page, the new post, and one old post. If anything is broken, tell me and offer to revert the merge.

## Done when

The new post is live at https://lcellentani.github.io/posts/what-eight-repos-taught-me/ and an old post still loads at its old URL.
