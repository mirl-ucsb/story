---
layout: default
title: Upgrade Summary
---

## Upgrade Summary
- **From:** 0.9.2-beta
- **To:** 0.9.3-beta
- **Date:** 2026-03-16
- **Automated changes:** 16
- **Manual steps:** 2

## Automated Changes Applied

### Configuration (1 file)

- [x] Updated _config.yml: version 0.9.3-beta (2026-03-16)

### Layouts (3 files)

- [x] Updated _layouts/object.html - Coordinate panel restyle, i18n, multi-page instructions
- [x] Updated _layouts/index.html - Smart thumbnail size selection for IIIF sizes array
- [x] Updated _layouts/objects-index.html - Smart thumbnail size selection for objects gallery

### Styles (3 files)

- [x] Updated _sass/_coordinate-panel.scss - New coordinate panel SCSS partial
- [x] Updated _sass/_viewer.scss - Portrait aspect ratio, page selector truncation fix
- [x] Updated assets/css/telar.scss - Add coordinate-panel import

### Scripts (6 files)

- [x] Updated scripts/iiif_utils.py - Fix scaleFactors, edge tiles, thumbnail generation order
- [x] Updated assets/js/telar-story.js - Rebuilt bundle with page switching fix
- [x] Updated assets/js/telar-story.js.map - Updated source map
- [x] Updated assets/js/telar-story/navigation.js - Page change detection in navigation
- [x] Updated assets/js/telar-story/viewer.js - Card recreation on page change
- [x] Updated scripts/telar/csv_utils.py - Page column case normalisation

### Other (3 files)

- [x] Updated _data/languages/en.yml - Add multi-page instruction key
- [x] Updated _data/languages/es.yml - Add multi-page instruction key, fix possessive
- [x] Updated CHANGELOG.md - Added v0.9.3-beta changelog entry

## Manual Steps Required

Please complete these after merging:

1. **If you use GitHub Pages:**

Your site will automatically regenerate IIIF tiles with the corrected info.json files when it rebuilds. To trigger a rebuild now, go to your repository's Actions tab, select the "Build and Deploy" workflow, and click **Run workflow**.
2. **If you work with your site locally:**

If your site uses self-hosted images, regenerate IIIF tiles to fix the info.json files. This corrects two issues: a crash for small images (under 512px) and incorrect edge tiles for larger images (over 1024px).

`python3 scripts/generate_iiif.py --base-url YOUR_SITE_URL`

(Replace YOUR_SITE_URL with your site's URL, e.g. https://yourusername.github.io/your-repo)

## Resources

- [Full Documentation](https://telar.org/docs)
- [CHANGELOG](https://github.com/UCSB-AMPLab/telar/blob/main/CHANGELOG.md)
- [Report Issues](https://github.com/UCSB-AMPLab/telar/issues)
