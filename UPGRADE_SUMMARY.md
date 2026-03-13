---
layout: default
title: Upgrade Summary
---

## Upgrade Summary
- **From:** 0.8.1-beta
- **To:** 0.9.2-beta
- **Date:** 2026-03-13
- **Automated changes:** 96
- **Manual steps:** 8

## Automated Changes Applied

### Configuration (6 files)

- [x] Reordered url before baseurl in _config.yml
- [x] Removed shared_url from _config.yml (no longer needed)
- [x] Updated _config.yml: version 0.9.0-beta (2026-03-13)
- [x] Added _includes/katex.html - KaTeX CDN loading and delimiter config
- [x] Updated _config.yml: version 0.9.1-beta (2026-03-13)
- [x] Updated _config.yml: version 0.9.2-beta (2026-03-13)

### Layouts (7 files)

- [x] Updated _layouts/index.html
- [x] Updated _layouts/objects-index.html
- [x] Updated _layouts/object.html
- [x] Updated _layouts/story.html
- [x] Updated _sass/_layout.scss
- [x] Updated _layouts/story.html - Dynamic KaTeX loading for stories with LaTeX
- [x] Updated _layouts/default.html - Conditional KaTeX loading (objects, glossary, custom pages)

### Includes (3 files)

- [x] Updated _includes/story-step.html
- [x] Updated scripts/telar/core.py - Include has_latex in story JSON metadata
- [x] Updated assets/js/telar-story.js - Rebuilt JS bundle (includes panels.js LaTeX changes)

### Styles (5 files)

- [x] Updated _sass/_mixins.scss
- [x] Updated _sass/_viewer.scss
- [x] Updated assets/css/telar.scss
- [x] Added _sass/_latex.scss - LaTeX styling overrides
- [x] Updated assets/css/telar.scss - Added LaTeX stylesheet import

### Scripts (31 files)

- [x] Updated scripts/iiif_utils.py
- [x] Updated scripts/process_pdf.py
- [x] Updated scripts/generate_iiif.py
- [x] Updated scripts/generate_collections.py
- [x] Updated scripts/fetch_google_sheets.py
- [x] Updated scripts/telar/core.py
- [x] Updated scripts/telar/csv_utils.py
- [x] Updated scripts/telar/processors/stories.py
- [x] Updated scripts/telar/processors/objects.py
- [x] Updated scripts/telar/images.py
- [x] Updated scripts/telar/glossary.py
- [x] Updated scripts/telar/markdown.py
- [x] Updated assets/js/telar-story/viewer.js
- [x] Updated assets/js/telar-story/navigation.js
- [x] Updated assets/js/telar-story/state.js
- [x] Updated assets/js/story-unlock.js
- [x] Updated assets/js/telar-story-bundle.js
- [x] Updated assets/js/telar-story.bundle.js
- [x] Updated scripts/README.md
- [x] Added scripts/telar/latex.py - LaTeX detection module (has_latex, protect/restore)
- [x] Updated scripts/telar/processors/stories.py - LaTeX detection in story content, extension fix
- [x] Updated scripts/telar/processors/objects.py - LaTeX detection in object descriptions, extension fix
- [x] Updated scripts/generate_collections.py - LaTeX detection in objects and glossary
- [x] Updated scripts/telar/markdown.py - LaTeX protection through markdown processing
- [x] Updated assets/js/telar-story/panels.js - LaTeX re-rendering after panel content injection
- [x] Updated assets/js/telar.js - LaTeX re-rendering after glossary content injection
- [x] Updated assets/js/story-unlock.js - Post-decryption KaTeX loading for encrypted stories
- [x] Updated assets/js/telar-story.js.map - Updated source map
- [x] Updated scripts/iiif_utils.py - Fix sizes array scanning, add 96px thumbnail
- [x] Updated scripts/generate_iiif.py - Updated version header
- [x] Updated scripts/process_pdf.py - Updated version header

### Documentation (7 files)

- [x] Removed placeholder directories (3d-models/, audio/, pdfs/) and README.md
- [x] Updated README.md
- [x] Updated telar-content/README.md
- [x] Updated telar-content/objects/README.md
- [x] Updated telar-content/spreadsheets/README.md
- [x] Updated telar-content/texts/README.md
- [x] Updated README.md - Updated version badge

### Other (37 files)

- [x] Moved components/images/ → telar-content/objects/
- [x] Moved components/structures/ → telar-content/spreadsheets/
- [x] Moved components/texts/ → telar-content/texts/
- [x] Removed components/ directory
- [x] Removed components/ from git tracking
- [x] Spreadsheets modified by user — keeping as-is
- [x] Updated .gitignore path references (components/ → telar-content/)
- [x] Updated _data/themes/trama.yml
- [x] Updated NOTICE
- [x] Updated _data/languages/en.yml
- [x] Updated _data/languages/es.yml
- [x] Updated _data/navigation.yml
- [x] Updated requirements.txt
- [x] Updated CHANGELOG.md
- [x] Updated LICENSE
- [x] Updated .gitignore
- [x] Updated tests/unit/test_image_processing.py
- [x] Fetched CSVs from Google Sheets
- [x] Added columns to objects.csv: year, object_type, subjects, featured
- [x] Added columns to project.csv: private
- [x] Added columns to story-1.csv: page
- [x] Created placeholder glossary.csv
- [x] Created telar-content/texts/glossary/example-term.md
- [x] Created telar-content/texts/glossary/ejemplo-termino.md
- [x] ⚠️  Found 8 reference(s) to old paths (components/) in your content:
- [x]   • telar-content/texts/stories/story1/step3-layer1.md: components/images/
- [x]   • telar-content/texts/stories/story1/step4-layer1.md: components/images/
- [x]   • telar-content/texts/stories/story1/step3-layer2.md: components/images/
- [x]   • telar-content/texts/stories/story1/step4-layer2.md: components/images/
- [x]   • telar-content/texts/stories/story1/step2-layer1.md: components/images/
- [x]   • telar-content/texts/stories/story1/step2-layer2.md: components/images/
- [x]   • telar-content/texts/stories/story1/step5-layer1.md: components/images/
- [x]   • telar-content/texts/stories/story1/step1-layer1.md: components/images/
- [x]   ℹ️  Update these references manually to telar-content/
- [x] Added tests/unit/test_latex_detection.py - LaTeX detection unit tests
- [x] Updated CHANGELOG.md - Added v0.9.1-beta changelog entry
- [x] Updated CHANGELOG.md - Added v0.9.2-beta changelog entry

## Manual Steps Required

Please complete these after merging:

1. **Update GitHub Actions workflow (required):**

Due to GitHub security restrictions, workflow files cannot be updated automatically.
Please replace your `.github/workflows/build.yml` with the latest version from the Telar repository.

**Important:** v0.9.0 adds `libvips-tools` installation for faster IIIF tile generation and updates all content path references from `components/` to `telar-content/`.

Steps:
1. Go to https://github.com/UCSB-AMPLab/telar/blob/main/.github/workflows/build.yml
2. Click the "Raw" button
3. Copy the entire file contents
4. Replace the contents of `.github/workflows/build.yml` in your repository ([guide](https://github.com/UCSB-AMPLab/telar/blob/main/.github/workflows/build.yml))
2. **If you use GitHub Pages:**

After updating the workflow file above, no further actions are needed. Your site will automatically rebuild with the new features.
3. **If you work with your site locally:**

1. **Regenerate IIIF tiles** (recommended — libvips is ~28x faster):

   Install libvips (one-time setup):
   - macOS: `brew install vips`
   - Ubuntu/Debian: `sudo apt-get install libvips-tools`

   Then regenerate tiles:
   ```
   python3 scripts/generate_iiif.py
   ```

   The script automatically uses libvips if available, falling back to the Python library.

2. **Optional — PDF support** (only if you want to add PDF documents):
   ```
   pip install PyMuPDF
   ```

3. **Rebuild your site:**
   ```
   python3 scripts/csv_to_json.py
   python3 scripts/generate_collections.py
   bundle exec jekyll build
   ```
4. **Check for broken path references:**

If you have hardcoded paths like `components/images/`, `components/structures/`, or `components/texts/` in your markdown files, custom pages, or HTML includes, these will break after the directory rename.

The migration script scans for common patterns and warns you, but please also review your custom content. Story CSV and objects CSV references are handled automatically by the framework — this only affects freeform markdown or HTML where you typed paths manually.

**Path mapping:**
- `components/images/` → `telar-content/objects/`
- `components/structures/` → `telar-content/spreadsheets/`
- `components/texts/` → `telar-content/texts/`
5. **Update Google Sheets columns (if you use Google Sheets):**

The migration automatically added any missing columns to your local CSV files. However, to keep these columns in future builds, you should also add them to your Google Sheets spreadsheet:

- **Story tabs**: Add a `page` column (after `zoom`) — for referencing specific pages of multi-page objects
- **Objects tab**: Add `year`, `object_type`, `subjects`, and `featured` columns — for gallery filtering and homepage featured objects
- **Project tab**: Add a `private` column — for password-protecting individual stories

You can also start from an updated template: https://bit.ly/telar-template ([guide](https://bit.ly/telar-template))
6. **What's new in v0.9.0:**

1. **Faster builds**: libvips tile generation is ~28x faster than the Python library
2. **Tify viewer**: Replaces UniversalViewer with a lighter, faster IIIF viewer
3. **PDF support**: Add PDF documents as objects — pages are automatically rendered as IIIF images
4. **Multi-page IIIF**: Story steps can reference specific pages of multi-page objects
5. **Trama theme**: New default theme with a fresh visual identity (your current theme is preserved)
6. **Simpler setup**: Only one Google Sheets URL needed (published_url)
7. **Custom metadata**: Extra columns in objects.csv are automatically displayed on object pages
7. Copy .github/workflows/telar-tests.yml and .github/workflows/build.yml from the latest Telar release. Workflow files cannot be updated automatically by the migration script due to GitHub Actions token permissions. The test workflow now only runs on the main Telar repos, not on user sites.
8. If your site uses self-hosted images, regenerate tiles to fix the info.json sizes array. Run your site's build workflow or run generate_iiif.py locally. This fixes tile rendering issues on Windows browsers.

## Resources

- [Full Documentation](https://telar.org/docs)
- [CHANGELOG](https://github.com/UCSB-AMPLab/telar/blob/main/CHANGELOG.md)
- [Report Issues](https://github.com/UCSB-AMPLab/telar/issues)
