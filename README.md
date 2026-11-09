# Cube Lab

Cube Lab is a browser-based twisty-puzzle playground. The app is delivered as a self-contained HTML page with no build step or external JavaScript/CSS dependencies.

## Features

- Interactive 3D cube and twisty-puzzle simulation
- Move controls, undo/redo, puzzle size and type selection
- Pattern/paint tools and tutorials
- Custom puzzle/part creation tools
- Scrambles and a speedcubing timer with solve history and averages
- Touch-friendly controls for phones and tablets
- Installable web-app metadata and an offline app-shell cache

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser. Most simulator features work directly from the file.
3. To test installability and offline caching, serve the folder over localhost (service workers require HTTPS or localhost). For example:

   ```bash
   python -m http.server 8000
   ```

4. Visit <http://localhost:8000>.

## Publish with GitHub Pages

1. Create a new GitHub repository and upload every file in this folder to the repository root.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and `/ (root)`, then save.
5. Wait for GitHub Pages to finish deploying; the Pages screen will show the public URL.

The site is configured to work from a repository subpath, so the default GitHub Pages project-site URL is supported.

## Files

| File | Purpose |
|---|---|
| `index.html` | Main Cube Lab application |
| `icon-192.png` | App icon for supported devices |
| `icon-512.png` | High-resolution app icon |
| `manifest.webmanifest` | Installable web-app metadata |
| `sw.js` | Service worker for app-shell caching |
| `.nojekyll` | Prevents GitHub Pages from running Jekyll processing |

## Notes

- The app stores settings and user-created data in the browser's local storage. Browser data is local to that browser/device and is not automatically synced between devices.
- Use HTTPS (GitHub Pages provides it) for service-worker and install features.
- No license has been added. Add a `LICENSE` file only after choosing the terms under which you want others to use, modify, and redistribute your work.
