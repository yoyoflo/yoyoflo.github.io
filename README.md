# Yosime Flood — Mathematics

Static academic website prepared for https://yoyoflo.github.io/.
All pages and PDFs are ready to publish; no Jekyll, Node.js, or build step is required.

## Publish on GitHub Pages

1. Create a **public** repository owned by `yoyoflo`, named exactly `yoyoflo.github.io`.
2. Upload the contents of this folder to the repository root on `main`. The root must contain `index.html`, not an extra enclosing folder.
3. In **Settings → Pages**, choose **Deploy from a branch**, branch **main**, folder **/ (root)**, and save.
4. Wait for the Pages deployment to succeed and visit https://yoyoflo.github.io/.

The public repository exposes the uploaded site files and PDFs. This package contains only website content and documentation, with no ChatGPT authentication or hosting configuration.

## Edit and upload work

- Home: `index.html`
- About: `about/index.html`
- Notes list: `notes/index.html`
- Projects list: `projects/index.html`
- Talks list: `talks/index.html`
- Solutions list: `solutions/index.html`
- CV placeholder: `cv/index.html`
- Shared styling: `assets/style.css`
- Thesis and talk overview pages: `work/<title>/index.html`

To add notes, upload a PDF into `notes/`, then copy an existing entry in `notes/index.html` and update its title, link, and description. Notes and solutions open PDFs directly; their navigation tabs open the corresponding index.

The header and profile sidebar are static HTML repeated on each page. If changing shared navigation or contact information, update it across all `index.html` files and `404.html`.

To replace a PDF without changing links, use the same filename. If its page count or description changes, update the corresponding list entry as well.

## Preview locally

From this folder run `python3 -m http.server 8000`, then open http://localhost:8000/.
Use this local server rather than opening HTML files directly, because links are relative to the website root.

## Migration notes

Prepared from the existing Sites source, version 20, commit fa78e04c569189f368f340aebe42396c373dd810.
The seven original PDFs were copied byte-for-byte, including the revised algebraic geometry contents page.
The minimalist page structure and content are preserved. Fonts use a system sans-serif fallback so no external font download is required. The profile photo and academic CV remain placeholders.
