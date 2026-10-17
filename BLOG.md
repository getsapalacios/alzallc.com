# Writing blog posts

Posts are Markdown files in `_posts/`, named `YYYY-MM-DD-short-title.md`.

## Private drafts
Write drafts in `_drafts/` (no date in the file name). That folder is in `.gitignore`,
so drafts stay on your Mac and never reach the public GitHub repo.

## Publish
1. Move the file from `_drafts/` to `_posts/` and add the date to its name.
2. Set `published: true` in its header (or remove the line).
3. Open a PR. Merging it puts the post live.

## Unpublish (hide a live post)
Set `published: false` in its header and merge. The page, its URL and its spot on
`/blog/` disappear on the next deploy (about a minute). To bring it back, set it to `true`.
To remove it for good, move it back to `_drafts/` instead.

## Preview locally
    jekyll serve --drafts --unpublished
Then open http://localhost:4000/blog/.
