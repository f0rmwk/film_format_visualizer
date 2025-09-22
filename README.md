# Film Format Visualizer

Interactive visualizer comparing common motion-picture film formats. This no-build setup runs directly in the browser using CDN scripts for React, ReactDOM, Tailwind, and Babel.

## Run locally

- Option 1: Open `index.html` directly in a browser.
- Option 2: Serve the folder (recommended for consistent asset loading):
  - Python: `python3 -m http.server 8000` then open `http://localhost:8000/`
  - Node (if installed): `npx serve .` and open the printed URL

## Development notes

- No bundler or package install required.
- React and Tailwind are loaded from CDNs.
- JSX is transpiled in the browser via Babel Standalone.
- The component source is in `film_format_overlay_visualizer_interactive.jsx`.

## Project structure

- `index.html` — Static entry page; mounts the visualizer.
- `film_format_overlay_visualizer_interactive.jsx` — React component (no-build compatible).
- `.gitignore` — Common ignores for macOS/Node projects.
- `.gitattributes` — Normalize line endings in Git.

## Git setup

Initialize a repo and make the first commit:

```bash
git init
git add .
git commit -m "Initialize Film Format Visualizer (no-build setup)"
```

(Optional) Set the default branch name:

```bash
git branch -M main
```

Then create a remote and push as needed.

## GitHub Pages

This repo includes a GitHub Actions workflow that publishes the site to GitHub Pages on every push to `main`.

- First push triggers the workflow automatically.
- Pages URL (once deployed): `https://f0rmwk.github.io/film_format_visualizer/`
- A `.nojekyll` file is included to ensure assets aren’t processed by Jekyll.

If Pages isn’t enabled automatically, in GitHub go to: Settings → Pages → Build and deployment → Source → GitHub Actions.
