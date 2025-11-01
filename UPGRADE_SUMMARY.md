---
layout: default
title: Upgrade Summary
---

## Upgrade Summary
- **From:** 0.3.1-beta
- **To:** 0.3.4-beta
- **Date:** 2025-11-01
- **Automated changes:** 28
- **Manual steps:** 2

## Automated Changes Applied

### Configuration (2 files)

- [x] Removed unused OpenSeadragon configuration section from _config.yml
- [x] Added telar_language configuration field to _config.yml

### Layouts (10 files)

- [x] Moved index.html to _layouts/index.html
- [x] Added _layouts/upgrade-summary.html
- [x] Updated story layout
- [x] Updated object layout
- [x] Updated objects index layout
- [x] Updated default layout
- [x] Updated glossary layout
- [x] Updated glossary index layout
- [x] Updated page layout
- [x] Updated index layout

### Includes (6 files)

- [x] Added _includes/upgrade-alert.html
- [x] Updated story-step include
- [x] Updated panels include
- [x] Updated viewer include
- [x] Updated header include
- [x] Updated footer include

### Styles (1 file)

- [x] Updated telar styles

### Scripts (3 files)

- [x] Added objects.json endpoint
- [x] Updated story JavaScript
- [x] Updated telar JavaScript

### Documentation (2 files)

- [x] Updated README
- [x] Updated docs README

### Other (4 files)

- [x] Created index.md in root directory
- [x] Added Python entries to .gitignore
- [x] Updated IIIF URL warning
- [x] Updated IIIF tile generator

## Manual Steps Required

Please complete these after merging:

~~1. Update GitHub Actions workflow file (.github/workflows/build.yml) - Replace with latest version from https://github.com/UCSB-AMPLab/telar/blob/main/.github/workflows/build.yml to remove deprecated cron schedule ([guide](https://ampl.clair.ucsb.edu/telar-docs/docs/2-workflows/upgrading/))~~ (done!)
2. (Optional) Customize index.md content to personalize your site ([guide](https://ampl.clair.ucsb.edu/telar-docs/docs/6-customization/3-home-page/))

## Resources

- [Full Documentation](https://ampl.clair.ucsb.edu/telar-docs)
- [CHANGELOG](https://github.com/UCSB-AMPLab/telar/blob/main/CHANGELOG.md)
- [Report Issues](https://github.com/UCSB-AMPLab/telar/issues)
