# markhare.org

A small personal site built with Jekyll and hosted on GitHub Pages. Posts are plain Markdown files; there is no JavaScript application or database to maintain.

## Publish a post

1. Copy `_posts/2026-09-08-welcome.md`.
2. Rename it using `YYYY-MM-DD-short-title.md`.
3. Update the title and description at the top, then write underneath in Markdown.
4. Commit and push. GitHub Pages republishes the site automatically.

Drafts can live in `_drafts/` (create the folder when needed). GitHub will ignore them until they are moved into `_posts/` and given a date-prefixed filename.

## Add a photo

Put the image in `assets/images/`, then add it to a post:

```markdown
![A useful description of the photograph](/assets/images/photo-name.jpg)
```

Resize large camera images before committing them. A width around 1600–2400 pixels and a compressed JPEG or WebP usually works well.

## Edit the site

- `_config.yml` controls the title, description, address, and URL format.
- `_layouts/` contains the shared page HTML.
- `assets/css/site.css` contains the visual design.
- `about.md` contains the About page.

## Preview locally (optional)

With Ruby and Bundler installed:

```sh
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.

