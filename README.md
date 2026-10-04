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
- Export PNG/JPG, copy to clipboard, native share sheet on mobile
- No build step, no tracking, nothing is uploaded

## Run locally
Export needs the page served over http (opening the file directly taints the canvas):

    python3 -m http.server 8000

then open http://localhost:8000

## Deploy on GitHub Pages
1. Push this folder to a new repo.
2. Settings > Pages > Deploy from branch > `main` / root.

Swap the default image by replacing `assets/default.png`.
