---
layout: default
title: Upgrade Summary
---

## Upgrade Summary
- **From:** 0.6.2-beta
- **To:** 0.7.0-beta
- **Date:** 2026-01-31
- **Automated changes:** 84
- **Manual steps:** 3

## Automated Changes Applied

### Configuration (4 files)

- [x] Updated _config.yml: version 0.6.3-beta (2026-01-31)
- [x] Updated scripts/telar/config.py
- [x] Updated vitest.config.js
- [x] Updated _config.yml: version 0.7.0-beta (2026-01-31)

### Layouts (2 files)

- [x] Updated _layouts/story.html
- [x] Updated _sass/_layout.scss

### Styles (9 files)

- [x] Updated _sass/_mixins.scss
- [x] Updated _sass/_typography.scss
- [x] Updated _sass/_panels.scss
- [x] Updated _sass/_widgets.scss
- [x] Updated _sass/_story.scss
- [x] Updated _sass/_embed.scss
- [x] Updated _sass/_share.scss
- [x] Updated _sass/_viewer.scss
- [x] Updated assets/css/telar.scss

### Scripts (36 files)

- [x] Updated scripts/csv_to_json.py - Inline content support, CSV parsing fix
- [x] Warning: Could not fetch assets/js/story.js
- [x] Removed deprecated file: assets/js/story.js
- [x] Added JavaScript build artifacts to .gitignore
- [x] Updated assets/js/telar-story/state.js
- [x] Updated assets/js/telar-story/utils.js
- [x] Updated assets/js/telar-story/viewer.js
- [x] Updated assets/js/telar-story/panels.js
- [x] Updated assets/js/telar-story/navigation.js
- [x] Updated assets/js/telar-story/main.js
- [x] Updated scripts/telar/__init__.py
- [x] Updated scripts/telar/csv_utils.py
- [x] Updated scripts/telar/images.py
- [x] Updated scripts/telar/iiif_metadata.py
- [x] Updated scripts/telar/glossary.py
- [x] Updated scripts/telar/widgets.py
- [x] Updated scripts/telar/markdown.py
- [x] Updated scripts/telar/demo.py
- [x] Updated scripts/telar/core.py
- [x] Updated scripts/telar/processors/__init__.py
- [x] Updated scripts/telar/processors/project.py
- [x] Updated scripts/telar/processors/objects.py
- [x] Updated scripts/telar/processors/stories.py
- [x] Updated scripts/csv_to_json.py
- [x] Updated scripts/generate_collections.py
- [x] Updated scripts/build_local_site.py
- [x] Updated scripts/discover_sheet_gids.py
- [x] Updated scripts/fetch_demo_content.py
- [x] Updated scripts/fetch_google_sheets.py
- [x] Updated scripts/generate_iiif.py
- [x] Updated scripts/upgrade.py
- [x] Updated tests/js/state.test.js
- [x] Updated tests/js/utils.test.js
- [x] Updated tests/js/viewer.test.js
- [x] Updated tests/js/panels.test.js
- [x] Updated package.json

### Documentation (1 file)

- [x] Updated README.md

### Other (32 files)

- [x] Created directory: tests
- [x] Created directory: tests/unit
- [x] Created directory: tests/e2e
- [x] Created directory: tests/js
- [x] Created directory: tests/fixtures
- [x] Created directory: assets/js/telar-story
- [x] Created directory: _sass
- [x] Added Python cache entries to .gitignore
- [x] Updated pytest.ini
- [x] Warning: Could not fetch tests/__init__.py
- [x] Warning: Could not fetch tests/unit/__init__.py
- [x] Warning: Could not fetch tests/e2e/__init__.py
- [x] Updated tests/e2e/conftest.py
- [x] Updated tests/unit/test_csv_utils.py
- [x] Updated tests/unit/test_column_processing.py
- [x] Updated tests/unit/test_inline_content.py
- [x] Updated tests/unit/test_google_sheets.py
- [x] Updated tests/unit/test_widget_parsing.py
- [x] Updated tests/unit/test_glossary_links.py
- [x] Updated tests/unit/test_iiif_metadata.py
- [x] Updated tests/unit/test_image_processing.py
- [x] Updated tests/unit/test_carousel_widget.py
- [x] Updated tests/unit/test_extract_credit.py
- [x] Updated tests/unit/test_project_processing.py
- [x] Updated tests/unit/test_apply_metadata.py
- [x] Updated tests/unit/test_process_widgets.py
- [x] Updated tests/unit/test_upgrade_utils.py
- [x] Updated tests/e2e/test_story_navigation.py
- [x] Updated tests/e2e/test_embed_mode.py
- [x] Updated tests/e2e/test_panel_interactions.py
- [x] Updated requirements.txt
- [x] Updated CHANGELOG.md

## Manual Steps Required

Please complete these after merging:

1. **Update GitHub Actions workflows:**

Due to GitHub security restrictions, workflow files cannot be updated automatically.
Please manually copy these files from the Telar repository:

1. `.github/workflows/build.yml` - Updated with Node.js setup and JS build step
2. `.github/workflows/upgrade.yml` - Updated version header
3. `.github/workflows/telar-tests.yml` - NEW: Runs Python and JavaScript tests

Download from: https://github.com/UCSB-AMPLab/telar/tree/main/.github/workflows ([guide](https://github.com/UCSB-AMPLab/telar/tree/main/.github/workflows))
2. **If you work with your site locally:**

Node.js is now required to build the JavaScript bundle. Install dependencies:

```
npm install
```

The build script now includes a JavaScript build step:

```
python3 scripts/build_local_site.py
```

Or build JavaScript separately:

```
npm run build:js
```
3. **Optional: Run the test suite locally**

This release includes 305 automated tests. To run them:

**Python tests (235 tests):**
```
python3 -m pytest tests/unit/ -v
```

**JavaScript tests (35 tests):**
```
npm run test:js
```

**E2E tests (35 tests) - requires Playwright:**
```
playwright install chromium
python3 -m pytest tests/e2e/ -v
```

## Resources

- [Full Documentation](https://telar.org/docs)
- [CHANGELOG](https://github.com/UCSB-AMPLab/telar/blob/main/CHANGELOG.md)
- [Report Issues](https://github.com/UCSB-AMPLab/telar/issues)
