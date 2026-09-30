# Fabric Planning Theme Studio

Design, check, and share one theme for every sheet in a Fabric Planning workspace. A single theme is previewed live on sample **Intelligence** reports, **Planning** sheets (Hierarchy, Table, Tree), and **PowerTable** layouts (Table, Gantt, Gantt resources, Calendar, Kanban).

Live: https://deepaklumel.github.io/fabric-theme-studio/

## What you can do

- **Start from a theme**: pick a built-in theme, or create one from a brand color, a Coolors palette, an image, theme JSON, or a short description.
- **Edit**: colors, page, visual elements, and font in the Properties pane, with undo/redo and per-section, per-tab, and full resets.
- **Check**: WCAG contrast check with one-click suggested fixes, and color vision simulation.
- **Share**: save to this browser, copy or download the theme JSON, or copy a share link.

## Theme JSON

The exported file is the Fabric Planning theme format (`label`, `themeType`, `theme.colors`, `theme.page`, `theme.elements`, `theme.typography`). It is not a Power BI report theme. Imported and shared themes are validated against the built-in defaults; missing or invalid settings fall back to defaults and unknown keys are kept, so a theme round-trips unchanged.

## Structure

```
index.html      entry point (studio chrome + sample sheets)
css/styles.css  all styles
js/icons.js     inline Fluent UI icons
js/app.js       all application logic
fonts/          embedded Segoe UI weights
favicon.svg     app icon
```

## Running locally

Static site, no build step or dependencies. Serve the folder with any static file server:

```
python3 -m http.server 8123
```

then open http://localhost:8123.

## Deploying

GitHub Pages deploys from the root of `main`; pushing to `main` updates the live site.
