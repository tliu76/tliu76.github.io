# Notes Site Starter

This folder is a standalone Jekyll notes site starter.

## 1. Create a new repo for notes

Use a repository like `YOUR-NOTES-SITE.github.io`.

## 2. Copy this starter

Copy everything in this folder to the root of that new repo.

## 3. Update site URL

Edit `_config.yml`:

```yml
url: "https://YOUR-NOTES-SITE.github.io"
baseurl: ""
```

## 4. Deploy with GitHub Pages

Push to `main` and enable GitHub Pages (Deploy from branch, root).

## 5. Connect your main site

In your main homepage repo (`tliu76.github.io`), set:

```yml
notes_site_url: "https://YOUR-NOTES-SITE.github.io"
```

Then your `/category/` page will jump to these notes pages.
