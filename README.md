# Laurent Juliá Calac — portfolio

Static site, no build step. Open `index.html` through a local server
(`python3 -m http.server 8000`) or publish it with GitHub Pages.

```
index.html          the whole page
css/style.css       palette, type, components (light + dark follow the system)
assets/
  Laurent_JuliaCalac_Resume_US.pdf   "Resume (US)" buttons
  Laurent_JuliaCalac_CV_EU.pdf       "CV (Europe)" buttons
  img/                               headshot, logos, project and tennis images
  img/originals/                     full-size photos (git-ignored)
```

## Adding a project image

Replace the `<span class="placeholder">…</span>` inside a card's `.media` with
`<img src="assets/img/ecg.png" alt="…">`, or a short muted clip:
`<video src="assets/img/tennis-ai.mp4" autoplay muted loop playsinline></video>`.
Resize large photos first: `sips -s format jpeg -Z 1400 in.png --out out.jpg`.

## Adding a project

Copy an `<article class="pcard">` block in `index.html`. Its `data-tags`
(`genai`, `dl`, `nlp`, `cv`) decide which filter buttons show it.

## Updating the resumes

Replace the two PDFs in `assets/`, keeping the file names.
