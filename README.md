# The Real Jetson — gallery site

Self-contained gallery: 38 photographs and 41 clips of Jetson, 2021–2026.
No build step, no dependencies. `index.html` plus the four asset folders is the whole site.

## Publish on GitHub Pages

1. Create a new public repository on github.com (suggested name: `jetson-gallery`).
2. Upload the entire contents of this folder to the repository root
   (GitHub Desktop handles the 400 MB of media most reliably; the web
   uploader caps out on batches this size).
3. In the repository: Settings → Pages → Source: "Deploy from a branch" →
   Branch: `main`, folder `/ (root)` → Save.
4. The site publishes at `https://YOURUSERNAME.github.io/jetson-gallery/`
   within a couple of minutes.

## Embed on brockalston.com (Wix)

Add an Embed → "Embed a site" element (same as the interactive map) and
point it at the Pages URL. Suggested sizing: full width, height 900 px on
desktop, with the element's own scrolling enabled so visitors can move
through the years inside the frame.

```
https://YOURUSERNAME.github.io/jetson-gallery/
```

## Notes

- Videos are poster-only until clicked, so initial page load is a few
  hundred kilobytes of thumbnails, not the 400 MB archive.
- Every file is under GitHub's 100 MB per-file limit.
- To add future items: drop the media into `img/`+`thumb/` or
  `vid/`+`poster/`, then add one card in `index.html` and one entry in
  the `ITEMS` array. Or bring the new files to a session and it gets
  done for you.
