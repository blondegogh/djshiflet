# DJ Shiflet

Portfolio site for DJ Shiflet, photographer.

## Structure

Single-file site — all HTML, CSS, and JS lives in `index.html`. No build step, no dependencies beyond a GSAP CDN import.

## Content

Images are served directly from Google Drive via thumbnail URLs. To update content, edit the data arrays at the top of the `<script>` block in `index.html`:

```js
const photographs = [ ... ]  // Shuffler + photographs viewer
const commissions = [ ... ]  // Commissions grid + detail viewer
const books       = [ ... ]  // Books grid + detail viewer
```

Each entry takes a Google Drive file ID. To get a file ID from a Drive share link:
`https://drive.google.com/file/d/FILE_ID_IS_HERE/view`

## Deployment

Hosted on Netlify. Connected to this repo — any push to `main` auto-deploys.

No build command. Publish directory: `/`

## Local development

Open `index.html` directly in a browser. No server required.
