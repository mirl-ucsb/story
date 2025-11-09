---
layout: default
title: Upgrade Summary
---

## Upgrade Summary
- **From:** 0.4.0-beta
- **To:** 0.4.1-beta
- **Date:** 2025-11-09
- **Automated changes:** 19
- **Manual steps:** 4

## Automated Changes Applied

### Configuration (1 file)

- [x] Restored WEBrick configuration comment

### Layouts (4 files)

- [x] Updated index layout (site description link styling)
- [x] Updated object layout (coordinate picker buttons)
- [x] Updated story layout (mobile responsive features restored)
- [x] Updated telar styles (mobile responsive features, gallery layout)

### Scripts (1 file)

- [x] Updated story JavaScript (mobile navigation, preloading, transitions)

### Documentation (1 file)

- [x] Updated README (supporter acknowledgments)

### Other (12 files)

- [x] Restored '# Story Interface Settings' header comment
- [x] Restored 'PLEASE DO NOT EDIT BELOW THIS LINE' warning
- [x] Restored '# Collections' header comment
- [x] Restored 'Collections Directory' comment
- [x] Restored '# Build Settings' header comment
- [x] Restored '# Defaults' header comment
- [x] Restored Jekyll dates comment
- [x] Restored 'Telar Settings' comment
- [x] Restored '# Plugins' header comment
- [x] Updated English language file with coordinate picker strings
- [x] Updated Spanish language file with coordinate picker strings
- [x] Updated CHANGELOG

## Manual Steps Required

Please complete these after merging:

1. Update your upgrade workflow file (one-time fix to prevent config comment deletion): (1) Go to https://raw.githubusercontent.com/UCSB-AMPLab/telar/main/.github/workflows/upgrade.yml (2) Select all (Ctrl/Cmd+A) and copy (3) In your repository, navigate to .github/workflows/upgrade.yml (4) Click the pencil icon to edit (5) Select all existing content and delete it (6) Paste the new content (7) Scroll to bottom and click "Commit changes". This fixes a bug that was stripping documentation comments from your _config.yml file during upgrades. ([guide](https://raw.githubusercontent.com/UCSB-AMPLab/telar/main/.github/workflows/upgrade.yml))
2. Run "bundle exec jekyll build" to test your upgraded site
3. Test mobile responsive features on small screens (optional)
4. Try the new coordinate picker buttons in object pages (optional)

## Resources

- [Full Documentation](https://ampl.clair.ucsb.edu/telar-docs)
- [CHANGELOG](https://github.com/UCSB-AMPLab/telar/blob/main/CHANGELOG.md)
- [Report Issues](https://github.com/UCSB-AMPLab/telar/issues)
