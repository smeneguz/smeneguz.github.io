# News & Event Photos

Photos and visual content for the News page. All images here are web-optimized
(max 1600 px long edge, JPEG quality ~80, EXIF rotation baked in). Full-resolution
originals are kept locally in `originals_photos_backup/` (git-ignored).

## Folder Organization

```
news/
├── conferences/       # Conference presentations and moments
│                      # COMPSAC 2023 Torino, COMPSAC 2025 Toronto,
│                      # ICSE 2026 Rio, COMPSAC 2026 Madrid
├── workshops/         # Workshop leadership and invited workshop talks
│                      # BlockDLT (COMPSAC), DLT Workshop (Pula 2026),
│                      # CrypTO Conference 2025 (Politecnico di Torino)
├── awards/            # Award ceremonies and recognitions
│                      # IEEE Certificate of Appreciation, COMPSAC 2026 Madrid
└── events/            # Other professional activities
                       # zkSummit14 Rome, DLT School Cagliari, Brunel London
                       # visiting period, seminars, PhD programme talks
```

## Naming Convention

`YYYY-MM_short-kebab-description.jpg` (month omitted when unknown).
The date is the date of the event, not of upload.

## Adding a Photo

1. Optimize before committing (keep files under ~400 KB):
   `python3` + Pillow: resize to max 1600 px, `ImageOps.exif_transpose`, save
   JPEG quality 80. Large phone photos (4-6 MB) slow the site down.
2. Place it in the right folder above with a dated name.
3. Reference it from `content/news.md` using the gallery markup:

```html
<div class="photo-grid">
  <figure class="photo-card">
    <img src="/images/news/conferences/2026-07_compsac-madrid-group.jpg"
         alt="Short description" loading="lazy">
    <figcaption>Caption with event, place, date.</figcaption>
  </figure>
</div>
```

Use `photo-grid` for 2-3 landscape images; add class `photo-grid--tall`
for portrait-oriented sets so rows stay compact.

## Captions: verify before writing

File names are not always reliable — several photos arrived labeled with the
wrong conference or year (e.g. a "COMPSAC_2026" file that was actually COMPSAC
2025 Toronto, a "BRAINS_2024_Paris" file that was a PhD programme talk).
Check what is visible in the photo (banners, slides, badges) before captioning.
