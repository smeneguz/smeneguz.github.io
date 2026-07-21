# News & Event Photos

This folder structure organizes photos and visual content for the news and announcements section of the profile.

## Folder Organization

```
news/
├── workshops/          # Photos from workshops and technical events
│                      # Examples: BlockDLT, Mentorium, Hands-on Ethereum Workshop
├── awards/            # Award ceremonies and recognition photos
│                      # Examples: Hackathon prizes, special recognitions
├── conferences/       # Conference presentations and moments
│                      # Examples: COMPSAC, ICSE, paper presentations
└── events/           # Other professional activities and events
                      # Examples: Research visits, seminars, collaborations
```

## Adding Photos

1. **Naming Convention**: Use descriptive names with dates
   - Format: `YYYY-MM-DD_description.jpg`
   - Example: `2024-07-15_compsac-osaka-presentation.jpg`

2. **Recommended Format**:
   - Format: JPG or PNG
   - Resolution: 1920×1080 minimum for best display
   - File size: Optimized for web (keep under 2MB)

3. **Adding to News**: Update `content/news.md` with photos and context
   ```markdown
   <img src="/images/news/workshops/2025-07-blockdlt-toronto.jpg" alt="BlockDLT 2025 Toronto" style="max-width: 100%; border-radius: 8px; margin: 1rem 0;">
   ```

## Photo Collections Needed

### Workshops & Technical Events
- [ ] BlockDLT 2024 (Osaka)
- [ ] BlockDLT 2025 (Toronto)  
- [ ] IEEE Mentorium 2025 (Toronto)
- [ ] IEEE Student Research Symposium 2025 (Toronto)
- [ ] Hands-on Ethereum Workshop (Torino, 2025)
- [ ] CrypTO SERICS Workshop (Torino, 2025)

### Awards & Recognition
- [ ] Blockstream Turin Simplicity Hackathon - 1st Prize (2024)
- [ ] IOTAxMasterZ Hackathon - Special Award (2024)
- [ ] IOTA Hackathon - 3rd Prize (Cagliari, 2024)

### Conferences
- [ ] COMPSAC 2024 (Osaka) - paper presentation moment
- [ ] COMPSAC 2025 (Toronto) - multiple presentations
- [ ] Other conference moments

### Professional Collaborations
- [ ] CITIC Research Week visits (Spain, 2024-2025)
- [ ] Brunel University London visiting researcher (2024-2025)
- [ ] Research team photos at Links Foundation
- [ ] University of Turin research activities

## Citation & Attribution

When adding photos, include:
- Date and location
- Event name
- Brief context/caption
- Any required photo credits

## Example Entry in news.md

```markdown
<div class="news-item-with-photo">
  <img src="/images/news/conferences/2024-07-compsac-osaka.jpg" alt="COMPSAC 2024 Osaka Presentation">
  <div class="news-content">
    <h3>COMPSAC 2024 Osaka: Paper Presentation</h3>
    <p>Presenting "Shaping the Future of Energy Markets" at IEEE COMPSAC in Osaka, Japan, July 2024.</p>
  </div>
</div>
```
