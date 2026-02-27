---
layout: default
title: Upgrade Summary
---

## Upgrade Summary
- **From:** 0.7.0-beta
- **To:** 0.8.1-beta
- **Date:** 2026-02-27
- **Automated changes:** 44
- **Manual steps:** 7

## Automated Changes Applied

### Configuration (6 files)

- [x] Added collection_interface section to _config.yml
- [x] Added show_on_homepage to story_interface in _config.yml
- [x] Renamed hide_stories to skip_stories in _config.yml
- [x] Renamed hide_collections to skip_collections in _config.yml
- [x] Updated _config.yml: version 0.8.0-beta (2026-02-27)
- [x] Updated _config.yml: version 0.8.1-beta (2026-02-27)

### Layouts (4 files)

- [x] Updated _layouts/story.html
- [x] Updated _layouts/index.html
- [x] Updated _layouts/objects-index.html
- [x] Updated _sass/_layout.scss

### Includes (2 files)

- [x] Updated _includes/share-panel.html
- [x] Updated _includes/header.html

### Styles (2 files)

- [x] Updated _sass/_share.scss
- [x] Updated _sass/_story.scss

### Scripts (19 files)

- [x] Added search-data.json to .gitignore
- [x] Updated scripts/telar/glossary.py
- [x] Updated scripts/generate_collections.py
- [x] Updated scripts/telar/encryption.py
- [x] Updated scripts/telar/processors/project.py
- [x] Updated scripts/telar/core.py
- [x] Updated assets/js/share-panel.js
- [x] Updated assets/js/story-unlock.js
- [x] Updated scripts/telar/csv_utils.py
- [x] Updated scripts/telar/search.py
- [x] Updated scripts/telar/iiif_metadata.py
- [x] Updated scripts/telar/processors/objects.py
- [x] Updated assets/js/objects-filter.js
- [x] Updated assets/js/lunr.min.js
- [x] Updated assets/js/telar-story/main.js
- [x] Updated scripts/fetch_google_sheets.py
- [x] Updated scripts/generate_collections.py
- [x] Updated scripts/telar/glossary.py
- [x] Updated scripts/telar/demo.py

### Documentation (2 files)

- [x] Updated README.md
- [x] Updated README.md

### Other (9 files)

- [x] Updated _data/languages/en.yml
- [x] Updated _data/languages/es.yml
- [x] Updated requirements.txt
- [x] Updated pytest.ini
- [x] Updated tests/unit/test_apply_metadata.py
- [x] Updated CHANGELOG.md
- [x] Updated _data/languages/en.yml
- [x] Updated _data/languages/es.yml
- [x] Updated CHANGELOG.md

## Manual Steps Required

Please complete these after merging:

1. **Update GitHub Actions workflows:**

Due to GitHub security restrictions, workflow files cannot be updated automatically.
Please manually copy these files from the Telar repository:

1. `.github/workflows/build.yml` - Updated with search data generation step

Download from: https://github.com/UCSB-AMPLab/telar/tree/main/.github/workflows ([guide](https://github.com/UCSB-AMPLab/telar/tree/main/.github/workflows))
2. **If you use GitHub Pages:**

No further actions needed beyond updating the workflow files above. Your site will automatically use the new features when it rebuilds.
3. **If you work with your site locally:**

A new Python dependency is required for protected stories:

```
pip install cryptography>=41.0.0
```

Or install all dependencies:

```
pip install -r requirements.txt
```
4. **New features available (optional):**

1. **Protected stories**: Add `protected` column to project.csv (yes/no) and set `story_key` in _config.yml
2. **Glossary CSV**: Create `components/structures/glossary.csv` as an alternative to individual markdown files
3. **Browse & search**: Automatically enabled on the objects page (disable with `browse_and_search: false` in _config.yml)
4. **Featured objects**: Set `show_sample_on_homepage: true` in _config.yml to show objects on the homepage

See the documentation for details on each feature.
5. **If you use GitHub Pages:**

No further actions needed. Your site will automatically use the new features when it rebuilds.
6. **If you work with your site locally:**

No new dependencies are required. Simply rebuild your site:

```
python3 scripts/csv_to_json.py
python3 scripts/generate_collections.py
bundle exec jekyll build
```
7. **What's new (no action required):**

1. **Spanish glossary tabs**: If your Google Sheet has a `glosario` tab, it will now be recognized and fetched correctly
2. **Demo content**: Demo objects now display with full gallery metadata (year, type, subjects) if you have demo content enabled
3. **Template update**: The Google Sheets template has been simplified from 8 to 6 tabs. If you'd like the latest template, visit https://bit.ly/telar-template

## Resources

- [Full Documentation](https://telar.org/docs)
- [CHANGELOG](https://github.com/UCSB-AMPLab/telar/blob/main/CHANGELOG.md)
- [Report Issues](https://github.com/UCSB-AMPLab/telar/issues)
