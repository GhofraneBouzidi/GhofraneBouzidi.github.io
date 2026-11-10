# Ghofrane Bouzidi - Portfolio

A single-page portfolio site. No build step, no dependencies, no server code.
Open `index.html` in a browser and it works.

## Files (keep them all together, in one flat folder)

| File | What it is |
|---|---|
| `index.html` | The entire site: HTML, CSS and JavaScript in one file |
| `ghofrane.webp` | Portrait, background already removed |
| `helmet.alpha.webm` | Intro video with true transparency (Chrome, Edge, Firefox) |
| `helmet.fallback.mp4` | Same intro for browsers without transparent video (Safari) |
| `p-escanor.webp` | ESCANOR dashboard |
| `p-orbit.webp` | ORBIT-SAGE ship detections |
| `p-pvhmi.webp` | PV supervision HMI |
| `p-lora.webp` | LoRa weather link |
| `p-tacho.webp` | Sensorless tachometer |
| `p-veronica2.webp` | Veronica, assistant robot |
| `p-award.webp` | PES TGM first place |

Do not rename the files or move them into subfolders; the page calls them by name.
Fonts load from Google Fonts, so an internet connection is needed for the exact look.

## Publishing

**Netlify (fastest):** app.netlify.com, sign in, drag this whole folder onto the
dashboard. Live in seconds on a free address you can rename.

**GitHub Pages:** create a public repo named `GhofraneBouzidi.github.io`, upload
these files to its root, then Settings -> Pages -> Deploy from branch `main`,
folder `/ (root)`. A minute later it is at https://ghofranebouzidi.github.io

**Custom domain:** buy a domain, then use the *Custom domain* setting on either
host. Both issue the HTTPS certificate free.

## Editing it later

- **Colours** - the `:root { ... }` block at the top. Change `--gold`,
  `--caramel`, `--beige` and the whole site follows.
- **French text** - every translatable element carries a `data-fr="..."`
  attribute. Edit that for the French wording; the English is the visible text.
- **Add a project** - copy an `<article class="pcard tilt rv">` block in the
  Projects section, or a `<div class="arch-row rv">` line in the archive list.
- **Swap a photo** - replace the `p-*.webp` file, keeping the same name.
- **Section glow** - each `<section>` has `data-h1` / `data-h2` / `data-h3`,
  colour-wheel angles (0-360) that set the aurora for that section.
- **The blueprint** - circuit symbols and formulas revealed around the cursor
  are drawn in the `sheet(c)` function near the bottom of the file.
