# In Bloom 🌿

A native garden website built as an interactive "yard sign" — sharing what's planted, what's been spotted, and why native plants matter.

## Pages

- **Home** (`index.html`) — garden overview and highlights
- **About** (`about.html`) — about the garden, plus a Q&A section
- **Resources** (`resources.html`) — books, organizations, and local resources for native gardening
- **Animal Sightings** (`animal-sightings.html`) — trail cam photos and wildlife video

## Tech

Plain HTML/CSS/JS with [Tailwind CSS](https://tailwindcss.com/) loaded via CDN. No build step, no dependencies to install — just open any `.html` file in a browser.

## Running locally

Clone the repo and open `index.html` directly in your browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deployment

This site is set up to deploy automatically to **GitHub Pages** via GitHub Actions on every push to `main`. See `.github/workflows/deploy.yml`.

To enable it on your repo:
1. Push this code to a GitHub repository.
2. Go to **Settings → Pages**.
3. Under "Build and deployment", set **Source** to "GitHub Actions".
4. Push a commit to `main` — the site will deploy automatically and the live URL will appear in the Pages settings (and in the Actions run summary).

## Editing content

- Update text and links directly in the relevant `.html` file.
- Add new images to the `Images/` folder and reference them with `Images/your-file.jpg`.
- For large photos, consider compressing before adding (keeping images under ~500KB each keeps the site fast).

## Notes

- The hummingbird clip is served as `Images/hummingbird.mp4` (re-encoded for broad browser support — the original `.MOV` format isn't reliably playable in all browsers).
