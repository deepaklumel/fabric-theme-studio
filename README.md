# Plan Theme Studio

A Power BI / Microsoft Fabric report-theme design tool. Build, preview, and export `.json` report themes with live previews across sample Intelligence, Planning, and PowerTable report pages.

## Structure

```
index.html      entry point
css/style.css   all styles
js/script.js    all application logic
fonts/          embedded Segoe UI weights (regular/semibold/bold)
favicon.svg     app icon
```

## Running locally

This is a static site with no build step or dependencies. Serve the folder with any static file server, e.g.:

```
npx serve .
```

or just open `index.html` directly in a browser (some features that fetch local files may require a server due to browser file:// restrictions).

## Deploying (GitHub Pages)

Push this folder to a GitHub repo and enable Pages (Settings → Pages → Deploy from branch → root), or push to a `gh-pages` branch.
