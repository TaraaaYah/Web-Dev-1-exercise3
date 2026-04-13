[README (3).md](https://github.com/user-attachments/files/26674569/README.3.md)
# J's Gallery

A clean, content-focused photography and video gallery website built with semantic HTML and CSS. Features a floated intro layout alongside a full-width gallery of images and video.

## Features

- **Full-width gallery rows** — flexbox rows where images and video scale equally to fill the viewport
- **Mixed media support** — seamlessly combines `<img>` and `<video>` elements in the same layout
- **Float-based intro** — right-floated hero image with text wrapping naturally around it
- **Serif typography** — Georgia font for an editorial, gallery-appropriate aesthetic
- **No dependencies** — pure HTML and CSS, no frameworks or build tools required

## Structure

```
index.html        # Main page (header, intro section, gallery rows)
styles.css        # All styles (sourced from J's_Gallery.txt)
```

## Layout Overview

### Header
Centred title and navigation bar with evenly spaced links (`justify-content: center; gap: 80px`). Max-width of 900px keeps it readable on wide screens.

### Intro Section
Text content with a right-floated image (`380 × 370px`, `object-fit: cover`). The section uses `overflow: hidden` to self-clear the float.

### Gallery
Full-width flexbox rows. Each item uses `flex: 1` to share width equally; video elements use `flex: 1.5` to give them slightly more prominence. All items share a fixed height of `250px` with `object-fit: cover` to crop without distortion.

## Colours

| Use | Value |
|---|---|
| Page background | `#d0d0d0` (light grey) |
| Nav links | `#0000ee` (browser default blue) |
| Visited links | `#551a8b` (browser default purple) |

## Typography

| Property | Value |
|---|---|
| Font family | `Georgia, serif` |
| H1 size | `3.5rem` |
| Body / nav | `1rem` |
| Line height | `1.6` |

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/js-gallery.git
   ```
2. Open `index.html` in your browser — no build step required.

## License

© J's Gallery. All rights reserved.
