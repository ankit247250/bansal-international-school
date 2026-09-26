# Bansal International School — live site

**https://ankit247250.github.io/bansal-international-school/**

This repository holds the **built, ready-to-serve** website — just static files.
There is no build step needed to deploy it: upload everything in this folder as-is.

## What's here

```
index.html                  entry point
assets/index-*.js           the React app, bundled and minified
assets/index-*.css          all styles, compiled from Tailwind
01.png                      hero photograph
02.png                      campus architectural sketch
BIS_logo.png                school logo
Icon_01..08.png             the eight "We Foster" icons
favicon.png                 browser tab icon
.nojekyll                   stops GitHub Pages running this through Jekyll
```

## Deploying to Hostinger (shared hosting / hPanel)

1. hPanel → **Files → File Manager**, open `public_html` for your domain.
2. Delete the default `default.php` / `index.html` placeholder Hostinger puts there.
3. Upload **the contents of this folder** (not the folder itself) into `public_html`.
   For uploads over ~100 MB or many files, use FTP or hPanel's Git deploy instead.
4. Visit your domain.

Nothing else is required — no Node, no npm, no database. The site is 100% static.

## Updating it later

Make your changes in the source repo, run `npm run build`, and re-upload the
`dist` folder. Or set up hPanel's **Git** feature to pull this repository
automatically on every push.

## Notes

- The `og:image` / `og:url` values in `index.html` are set to the current
  GitHub Pages address. Change them to your domain when you go live so link
  previews are correct.
- `assets/index-*.js` and `assets/index-*.css` have content hashes in their
  filenames, so they can be cached aggressively and forever.
