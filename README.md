# Everlyn International website

A static one-page site for Everlyn International: high-purity swimming pool salt exported from India for resorts, hotels and water treatment companies.

There is no build step. `index.html` is the page; `assets/` holds its styles, scripts, logo, intro film and photographs; `credits.html` lists the photograph licences.

## Run it locally

Serve the folder with any static server, for example:

```
python -m http.server 8000
```

Then open http://localhost:8000.

## Deploy

Vercel serves the folder as-is (see `vercel.json`: no framework, no install, no build).

## Still to replace

- `quotes@everlyn.example` and `hello@everlyn.example` in `index.html`: the real email addresses, or a form service on the quote form's `data-endpoint`.
- The stand-in photographs in `assets/img/` (credited in `credits.html`).
