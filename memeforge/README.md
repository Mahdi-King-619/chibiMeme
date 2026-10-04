# ChibiMeme

A layer-based meme editor that runs entirely in the browser. Default frame: Maomao and Jinshi (chibi).

## Features
- Unlimited draggable text and emoji layers (move, resize with the mouse wheel, rotate, outline, text box, CAPS)
- Caption-bar mode (white banner on top, modern meme style)
- Crop ratios: original, 1:1, 16:9, 9:16, 5:4
- Image filters: brightness, contrast, saturation, grayscale, blur, plus Deep fry and Noir
- Quick styles: classic top/bottom, subtitle, caption bar, reaction, and a "Surprise me" caption shuffler
- Undo/redo, keyboard shortcuts (arrows nudge, Del removes, Ctrl+D duplicates)
- Upload, drag-and-drop or paste any image to replace the background
- Save memes as PNG or JPG
- Copy PNGs to the clipboard when supported by the browser; use Save PNG if clipboard access is unavailable
- Share through the native share sheet on supported mobile browsers
- No build step, no tracking, nothing is uploaded

## Run locally
Open the folder through HTTP to enable image export. Opening `index.html` directly with a `file://` URL can block PNG/JPG export because the browser restricts access to local image files. Clipboard copy and native sharing also depend on browser support and a secure context (`localhost` or HTTPS).

From the repository root, run:

    py -m http.server 8000

Then open `http://localhost:8000`. On systems without the `py` launcher, use `python -m http.server 8000` or `python3 -m http.server 8000`.

## Deploy on GitHub Pages
1. Push this folder to a new repo.
2. Settings > Pages > Deploy from branch > `main` / root.

Swap the default image by replacing `assets/default.png`.
