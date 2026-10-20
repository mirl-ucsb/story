---
layout: default
title: Upgrade Summary
---

## Upgrade Summary
- **From:** 0.9.3-beta
- **To:** 1.8.1
- **Date:** 2026-10-12
- **Automated changes:** 598
- **Manual steps:** 36

## Automated Changes Applied

### Configuration (49 files)

- [x] Updated requirements.txt - Add PyMuPDF for PDF IIIF tile generation
- [x] Updated _config.yml: version 0.9.4-beta (2026-03-18)
- [x] Updated package.json - npm dependencies
- [x] Updated _data/languages/en.yml - English strings (clip_picker keys added)
- [x] Updated _data/languages/es.yml - Spanish strings (clip_picker keys added)
- [x] Updated _config.yml: max_viewer_cards 10 -> 8
- [x] Updated _config.yml: version 1.0.0-beta (2026-03-25)
- [x] Updated _data/languages/en.yml - English strings (collection_mode_heading added)
- [x] Updated _data/languages/es.yml - Spanish strings (collection_mode_heading added)
- [x] Added collection_mode: false to _config.yml (after telar_language)
- [x] Updated _config.yml: version 1.1.0 (2026-04-13)
- [x] Updated _data/languages/en.yml - English strings (sections_heading, back_to_start added)
- [x] Updated _data/languages/es.yml - Spanish strings (sections_heading, back_to_start added)
- [x] Updated _config.yml: version 1.2.0 (2026-04-16)
- [x] Updated _config.yml: version 1.2.1 (2026-05-08)
- [x] Updated _data/languages/en.yml — English language pack (new keys: glossary_intro, index_page.welcome, etc.)
- [x] Updated _data/languages/es.yml — Spanish language pack
- [x] Updated _config.yml: version 1.3.0 (2026-05-10)
- [x] Updated _data/languages/en.yml
- [x] Updated _data/languages/es.yml
- [x] Updated .gitignore — track assets/vendor/, ignore stale story bundles
- [x] Updated _data/languages/en.yml
- [x] Updated _data/languages/es.yml
- [x] Skipped .gitignore (assets/vendor/ already tracked)
- [x] Updated _data/languages/en.yml
- [x] Updated _data/languages/es.yml
- [x] Updated _data/languages/en.yml
- [x] Updated _data/languages/es.yml
- [x] Build workflow concurrency group: add the `concurrency` block to .github/workflows/build.yml by hand (or recopy the file). The in-Actions upgrade cannot modify workflow files; the Telar Compositor applies it automatically. See the manual step below.
- [x] Updated _data/katex.yml
- [x] Updated _data/languages/en.yml
- [x] Updated _data/languages/es.yml
- [x] Updated package.json
- [x] Updated package.json
- [x] Updated package-lock.json
- [x] Removed .github/dependabot.yml — dependency-bump pull requests are now managed by the Telar release process, not per-site
- [x] Updated requirements.txt
- [x] Updated package.json
- [x] Updated package-lock.json
- [x] Added _data/telar-build/ to .gitignore — the story page manifest generate_collections.py writes there is build output, regenerated on every build
- [x] Updated requirements.txt
- [x] Updated package.json
- [x] Updated package-lock.json
- [x] Updated _data/glossary_kinds.yml
- [x] Updated _data/languages/en.yml
- [x] Updated _data/languages/es.yml
- [x] Added tests/, pytest.ini, vitest.config.js, telar-content/texts/ to `exclude:` in _config.yml, so Jekyll does not publish them as pages of your site
- [x] Updated package.json
- [x] Updated package-lock.json

### Layouts (49 files)

- [x] Updated _layouts/story.html - Card-stack story layout
- [x] Updated _layouts/default.html - Default layout (CDN links removed)
- [x] Updated _layouts/object.html - Object page with video/audio support
- [x] Updated _layouts/objects-index.html - Gallery with media type thumbnails
- [x] Updated _layouts/index.html - Homepage with media-type-aware thumbnails
- [x] Updated _layouts/index.html - Homepage with collection mode branch
- [x] Updated _layouts/index.html - Homepage (ordinal number removal)
- [x] Updated _layouts/story.html - Story layout (section TOC, Back to Start button)
- [x] Updated _layouts/object.html - Object layout (ordinal removal from related stories)
- [x] Updated _layouts/index.html — Homepage layout (i18n fall-through + empty_states + JS i18n)
- [x] Updated _layouts/objects-index.html — Objects index layout (errors + empty_states wiring)
- [x] Updated _layouts/glossary-index.html — Glossary index layout (empty_states wiring)
- [x] Updated _layouts/story.html
- [x] Updated _layouts/object.html
- [x] Updated _layouts/default.html
- [x] Updated _layouts/default.html
- [x] Updated _layouts/index.html
- [x] Updated _layouts/object.html
- [x] Updated _layouts/story.html
- [x] Updated _layouts/story.html
- [x] Updated _layouts/index.html
- [x] Updated _layouts/default.html
- [x] Updated _layouts/index.html
- [x] Updated _layouts/object.html
- [x] Updated _layouts/objects-index.html
- [x] Updated _layouts/glossary-index.html
- [x] Updated _layouts/glossary.html
- [x] Updated _layouts/upgrade-summary.html
- [x] Updated _layouts/default.html
- [x] Updated _layouts/glossary.html
- [x] Updated _layouts/index.html
- [x] Updated _layouts/object.html
- [x] Updated _layouts/objects-index.html
- [x] Updated _layouts/story-fragment.html
- [x] Updated _layouts/story.html
- [x] Updated _layouts/upgrade-summary.html
- [x] Updated _layouts/index.html
- [x] Updated _layouts/object.html
- [x] Updated _layouts/objects-index.html
- [x] Updated _layouts/default.html
- [x] Updated _layouts/glossary-index.html
- [x] Updated _layouts/glossary.html
- [x] Updated _layouts/object.html
- [x] Updated _layouts/objects-index.html
- [x] Updated _layouts/story.html
- [x] Updated _layouts/index.html
- [x] Updated _layouts/object.html
- [x] Updated _layouts/objects-index.html
- [x] Updated _layouts/story.html

### Includes (52 files)

- [x] Updated _includes/story-step.html - Story step with clip and alt data
- [x] Updated _includes/panels.html - Panels (z-index consolidated)
- [x] Updated _includes/share-button.html - Share button (Lucide SVG)
- [x] Updated _includes/share-panel.html - Share panel (Lucide SVGs)
- [x] Updated _includes/panels.html - Panels with data-telar-panel attributes
- [x] Updated _includes/share-panel.html - Share panel with "this view" tab
- [x] Updated _includes/widgets/bibliography.html - Bibliography widget template (new)
- [x] Updated _includes/iiif-url-warning.html — IIIF URL warning (now references lang.errors.iiif_mismatch)
- [x] Updated _includes/viewer.html
- [x] Updated _includes/iiif-url-warning.html
- [x] Updated _includes/katex.html
- [x] Updated _includes/panels.html
- [x] Updated _includes/footer.html
- [x] Updated _includes/story-step.html
- [x] Updated _includes/viewer.html
- [x] Updated _includes/header.html
- [x] Updated _includes/iiif-url-warning.html
- [x] Updated _includes/katex.html
- [x] Updated _includes/object-grid-item.html
- [x] Updated _includes/panels.html
- [x] Updated _includes/share-embed-controls.html
- [x] Updated _includes/share-panel.html
- [x] Updated _includes/share-site-tab.html
- [x] Updated _includes/story-steps.html
- [x] Updated _includes/upgrade-alert.html
- [x] Updated _includes/widgets/accordion.html
- [x] Updated _includes/widgets/bibliography.html
- [x] Updated _includes/widgets/carousel.html
- [x] Updated _includes/widgets/tabs.html
- [x] Removed dead file _includes/viewer.html
- [x] Updated _includes/iiif-url-warning.html
- [x] Updated _includes/footer.html
- [x] Updated _includes/katex.html
- [x] Updated _includes/katex-loader.html
- [x] Updated _includes/panels.html
- [x] Updated _includes/share-panel.html
- [x] Updated _includes/story-step.html
- [x] Updated _includes/story-steps.html
- [x] Updated _includes/glossary-intro.html
- [x] Updated _includes/glossary-kind-entries.html
- [x] Updated _includes/glossary-kind-text.html
- [x] Updated _includes/glossary-kinds-used.html
- [x] Updated _includes/glossary-kinds.html
- [x] Updated _includes/widgets/glossary.html
- [x] Updated _includes/objects/metadata/audio.html
- [x] Updated _includes/objects/metadata/image.html
- [x] Updated _includes/objects/metadata/video.html
- [x] Updated _includes/objects/tools/audio.html
- [x] Updated _includes/objects/tools/image.html
- [x] Updated _includes/objects/tools/video.html
- [x] Updated _includes/story-step.html
- [x] Updated _includes/iiif-url-warning.html

### Styles (50 files)

- [x] Updated _sass/_story.scss - Card-stack story styles
- [x] Updated _sass/_viewer.scss - Object page viewer styles
- [x] Updated _sass/_panels.scss - Panel styles
- [x] Updated _sass/_share.scss - Share button styles
- [x] Updated _sass/_embed.scss - Embed mode styles
- [x] Updated _sass/_layout.scss - Layout styles (gallery thumbnails)
- [x] Updated _sass/_layout.scss - Layout styles (collection mode)
- [x] Updated _sass/_panels.scss - Panel styles (bibliography max-width)
- [x] Updated _sass/_story.scss - Story styles (title cards)
- [x] Updated _sass/_viewer.scss - Viewer styles (Tify background fix)
- [x] Updated _sass/_widgets.scss - Widget styles (bibliography hanging indent)
- [x] Updated _sass/_story.scss - Story styles (TOC, title card layer2 bg, Back to Start)
- [x] Updated assets/css/telar.scss
- [x] Updated _sass/_responsive.scss
- [x] Updated _sass/_story.scss
- [x] Updated _sass/_layout.scss
- [x] Updated _sass/_panels.scss
- [x] Updated _sass/_share.scss
- [x] Updated _sass/_embed.scss
- [x] Updated _sass/_viewer.scss
- [x] Updated _sass/_mixins.scss
- [x] Updated _sass/_coordinate-panel.scss
- [x] Updated _sass/_typography.scss
- [x] Updated _sass/_widgets.scss
- [x] Updated _sass/_story.scss
- [x] Updated _sass/_layout.scss
- [x] Updated _sass/_embed.scss
- [x] Updated _sass/_latex.scss
- [x] Updated _sass/_layout.scss
- [x] Updated _sass/_mixins.scss
- [x] Updated _sass/_panels.scss
- [x] Updated _sass/_responsive.scss
- [x] Updated _sass/_share.scss
- [x] Updated _sass/_story.scss
- [x] Updated _sass/_viewer.scss
- [x] Updated _sass/_widgets.scss
- [x] Updated assets/css/telar.scss
- [x] Updated _sass/_coordinate-panel.scss
- [x] Updated _sass/_embed.scss
- [x] Updated _sass/_latex.scss
- [x] Updated _sass/_layout.scss
- [x] Updated _sass/_mixins.scss
- [x] Updated _sass/_panels.scss
- [x] Updated _sass/_responsive.scss
- [x] Updated _sass/_share.scss
- [x] Updated _sass/_story.scss
- [x] Updated _sass/_typography.scss
- [x] Updated _sass/_viewer.scss
- [x] Updated _sass/_widgets.scss
- [x] Updated assets/css/telar.scss

### Scripts (352 files)

- [x] Updated assets/js/telar-icons.js - Lucide SVG icon module
- [x] Updated assets/js/embed.js - Embed mode (Lucide icons)
- [x] Updated assets/js/objects-filter.js - Gallery filter (media_type/medium)
- [x] Updated assets/js/share-panel.js - Share panel (Lucide icons)
- [x] Updated assets/js/story-unlock.js - Password unlock (Lucide icons)
- [x] Updated assets/js/telar-story.js - Bundled story JS
- [x] Updated assets/js/telar-story.js.map - Source map
- [x] Updated assets/js/telar-story/main.js - Story entry point
- [x] Updated assets/js/telar-story/card-pool.js - Card pool manager
- [x] Updated assets/js/telar-story/card-type.js - Card type detection
- [x] Updated assets/js/telar-story/iiif-card.js - IIIF card module
- [x] Updated assets/js/telar-story/text-card.js - Text card module
- [x] Updated assets/js/telar-story/scroll-engine.js - Scroll engine
- [x] Updated assets/js/telar-story/video-card.js - Video card module
- [x] Updated assets/js/telar-story/audio-card.js - Audio card module
- [x] Updated assets/js/telar-story/navigation.js - Navigation module
- [x] Updated assets/js/telar-story/state.js - Shared state
- [x] Updated assets/js/telar-story/viewer.js - Viewer module
- [x] Updated assets/js/telar-story/utils.js - Shared utilities
- [x] Updated assets/js/telar-story/panels.js - Panel module
- [x] Updated scripts/process_audio.py - Audio build pipeline
- [x] Updated scripts/build_local_site.py - Local build script (7-step)
- [x] Updated scripts/generate_collections.py - Collections generator
- [x] Updated scripts/generate_iiif.py - IIIF tile generator
- [x] Updated scripts/telar/core.py - CSV-to-JSON core
- [x] Updated scripts/telar/csv_utils.py - CSV utilities
- [x] Updated scripts/telar/processors/objects.py - Object processor
- [x] Updated scripts/telar/processors/stories.py - Story processor
- [x] Updated scripts/telar/search.py - Search data generator
- [x] Updated tests/js/card-pool.test.js - Card pool tests
- [x] Updated tests/js/card-type.test.js - Card type tests
- [x] Updated tests/js/iiif-card.test.js - IIIF card tests
- [x] Updated tests/js/iiif-lerp.test.js - IIIF lerp tests
- [x] Updated tests/js/text-card.test.js - Text card tests
- [x] Updated tests/js/scroll-engine.test.js - Scroll engine tests
- [x] Updated tests/js/navigation.test.js - Navigation tests
- [x] Updated tests/js/video-card.test.js - Video card tests
- [x] Updated tests/js/audio-card.test.js - Audio card tests
- [x] Updated tests/js/state.test.js - State tests
- [x] Updated tests/js/utils.test.js - Utils tests
- [x] Updated tests/unit/test_csv_utils.py - CSV utils tests
- [x] Updated tests/unit/test_generate_collections.py - Collections tests
- [x] Updated tests/unit/test_process_audio.py - Audio pipeline tests
- [x] Updated assets/js/share-panel.js - Share panel (deep link support)
- [x] Updated assets/js/telar-story.js - Bundled story JS
- [x] Updated assets/js/telar-story.js.map - Source map
- [x] Updated assets/js/telar-story/main.js - Story entry point (deep link init)
- [x] Updated assets/js/telar-story/card-pool.js - Card pool (title cards, media deactivation)
- [x] Updated assets/js/telar-story/deep-link.js - Deep linking module (new)
- [x] Updated assets/js/telar-story/navigation.js - Navigation (panel keyboard scroll, hash writes)
- [x] Updated assets/js/telar-story/panels.js - Panels (glossary deep-link numbers, hash writes)
- [x] Updated assets/js/telar-story/scroll-engine.js - Scroll engine (panel fix, hash writes)
- [x] Updated scripts/telar/core.py - Build pipeline (audio manifest generation)
- [x] Updated scripts/telar/widgets.py - Widget parser (bibliography support)
- [x] Updated tests/js/card-pool.test.js - Card pool tests (title cards)
- [x] Updated tests/unit/test_bibliography_widget.py - Bibliography widget tests (new)
- [x] Updated assets/js/telar-story.js - Bundled story JS
- [x] Updated assets/js/telar-story.js.map - Source map
- [x] Updated assets/js/telar-story/main.js - Story entry point (TOC links, Back to Start wiring)
- [x] Updated assets/js/telar-story/deep-link.js - Deep linking (navigateToStep, navigateToIntro, parent panel fix)
- [x] Updated assets/js/telar-story/navigation.js - Navigation (onStepChange callback)
- [x] Updated assets/js/telar-story/scroll-engine.js - Scroll engine (onStepChange callback)
- [x] Updated scripts/generate_collections.py - Collections (show_sections frontmatter, ordinal removal)
- [x] Updated scripts/telar/processors/project.py - Project processor (show_sections column)
- [x] Updated scripts/telar/csv_utils.py - CSV utils (mostrar_secciones alias)
- [x] Updated scripts/fetch_demo_content.py - Demo content fetcher (v-prefix tolerance fix)
- [x] Updated scripts/generate_collections.py — Sister-file localization for pages/ (about.md/acerca.md)
- [x] Updated assets/vendor/openseadragon.min.js
- [x] Updated assets/js/telar-story.js
- [x] Updated assets/js/telar-story.js.map
- [x] Updated assets/js/telar-story/iiif-manifest.js
- [x] Updated assets/js/telar-story/iiif-viewer.js
- [x] Updated assets/js/telar-story/layout-mode.js
- [x] Updated assets/js/telar-story/test-hook.js
- [x] Updated assets/js/telar-story/card-pool.js
- [x] Updated assets/js/telar-story/iiif-card.js
- [x] Updated assets/js/telar-story/main.js
- [x] Updated assets/js/telar-story/state.js
- [x] Updated assets/js/telar-story/scroll-engine.js
- [x] Updated assets/js/telar-story/audio-card.js
- [x] Updated assets/js/telar-story/video-card.js
- [x] Updated assets/js/telar-story/deep-link.js
- [x] Updated assets/js/telar-story/text-card.js
- [x] Updated assets/js/telar-story/viewer.js
- [x] Updated assets/js/telar-story/navigation.js
- [x] Updated scripts/iiif_utils.py
- [x] Updated scripts/README.md
- [x] Removed stale bundle file assets/js/telar-story.bundle.js
- [x] Removed stale bundle file assets/js/telar-story-bundle.js
- [x] Updated scripts/pipeline_utils.py
- [x] Updated scripts/telar/media_type.py
- [x] Updated scripts/discover_sheet_gids.py
- [x] Updated scripts/fetch_google_sheets.py
- [x] Updated scripts/fetch_demo_content.py
- [x] Updated scripts/generate_collections.py
- [x] Updated scripts/generate_iiif.py
- [x] Updated scripts/iiif_utils.py
- [x] Updated scripts/process_audio.py
- [x] Updated scripts/process_pdf.py
- [x] Updated scripts/telar/core.py
- [x] Updated scripts/telar/csv_utils.py
- [x] Updated scripts/telar/encryption.py
- [x] Updated scripts/telar/glossary.py
- [x] Updated scripts/telar/markdown.py
- [x] Updated scripts/telar/search.py
- [x] Updated scripts/telar/widgets.py
- [x] Updated scripts/telar/processors/objects.py
- [x] Updated scripts/telar/processors/project.py
- [x] Updated scripts/telar/processors/stories.py
- [x] Updated assets/vendor/wavesurfer/wavesurfer.min.js
- [x] Updated assets/vendor/wavesurfer/plugins/regions.min.js
- [x] Updated assets/js/telar-story.js
- [x] Updated assets/js/telar-story.js.map
- [x] Updated assets/js/telar-story/audio-card.js
- [x] Updated assets/js/telar-story/card-pool.js
- [x] Updated assets/js/telar-story/deep-link.js
- [x] Updated assets/js/telar-story/iiif-card.js
- [x] Updated assets/js/telar-story/iiif-viewer.js
- [x] Updated assets/js/telar-story/panels.js
- [x] Updated assets/js/telar-story/scroll-engine.js
- [x] Updated assets/js/telar-story/state.js
- [x] Updated assets/js/telar-story/utils.js
- [x] Updated assets/js/telar-story/video-card.js
- [x] Updated assets/js/telar-story/viewer.js
- [x] Updated assets/js/share-panel.js
- [x] Updated assets/js/story-unlock.js
- [x] Updated assets/js/objects-filter.js
- [x] Updated assets/js/embed.js
- [x] Updated assets/js/telar.js
- [x] Updated scripts/telar/glossary.py
- [x] Updated scripts/telar/processors/stories.py
- [x] Updated scripts/telar/core.py
- [x] Updated assets/js/telar.js
- [x] Updated scripts/telar/glossary.py
- [x] Updated assets/js/telar-story.js
- [x] Updated assets/js/telar-story.js.map
- [x] Updated assets/js/telar-story/audio-card.js
- [x] Updated assets/js/telar-story/card-pool.js
- [x] Updated assets/js/telar-story/deep-link.js
- [x] Updated assets/js/telar-story/iiif-card.js
- [x] Updated assets/js/telar-story/iiif-viewer.js
- [x] Updated assets/js/telar-story/main.js
- [x] Updated assets/js/telar-story/navigation.js
- [x] Updated assets/js/telar-story/panels.js
- [x] Updated assets/js/telar-story/scroll-engine.js
- [x] Updated assets/js/telar-story/state.js
- [x] Updated assets/js/telar-story/test-hook.js
- [x] Updated assets/js/telar-story/text-card.js
- [x] Updated assets/js/telar-story/utils.js
- [x] Updated assets/js/telar-story/video-card.js
- [x] Updated assets/js/telar-story/viewer.js
- [x] Updated assets/js/christmas-tree-decorator.js
- [x] Updated assets/js/embed.js
- [x] Updated assets/js/iiif-thumbnails.js
- [x] Updated assets/js/iiif-url-warning.js
- [x] Updated assets/js/katex-loader.js
- [x] Updated assets/js/object-theme.js
- [x] Updated assets/js/objects-filter.js
- [x] Updated assets/js/share-panel.js
- [x] Updated assets/js/story-unlock.js
- [x] Updated assets/js/telar.js
- [x] Updated assets/js/video-embed.js
- [x] Updated assets/js/wavesurfer-loader.js
- [x] Updated assets/js/widgets.js
- [x] Updated scripts/build_local_site.py
- [x] Updated scripts/csv_to_json.py
- [x] Updated scripts/discover_sheet_gids.py
- [x] Updated scripts/encrypt_protected_stories.py
- [x] Updated scripts/fetch_google_sheets.py
- [x] Updated scripts/generate_collections.py
- [x] Updated scripts/generate_iiif.py
- [x] Updated scripts/iiif_utils.py
- [x] Updated scripts/process_audio.py
- [x] Updated scripts/process_pdf.py
- [x] Updated scripts/telar/__init__.py
- [x] Updated scripts/telar/core.py
- [x] Updated scripts/telar/csv_utils.py
- [x] Updated scripts/telar/demo.py
- [x] Updated scripts/telar/encryption.py
- [x] Updated scripts/telar/iiif_metadata.py
- [x] Updated scripts/telar/markdown.py
- [x] Updated scripts/telar/media_type.py
- [x] Updated scripts/telar/processors/objects.py
- [x] Updated scripts/telar/processors/stories.py
- [x] Updated scripts/telar/search.py
- [x] Updated scripts/telar/widgets.py
- [x] Updated assets/js/README.md
- [x] Removed dead file assets/js/telar-icons.js
- [x] Upgrade-chain wiring fix (internal): the v1.5.4 -> v1.6.0 migration is now registered in scripts/upgrade.py, so upgrades starting below v1.6.0 no longer stop early at 1.5.4. No files in this site changed.
- [x] Updated assets/js/README.md
- [x] Updated assets/js/home-page.js
- [x] Updated assets/js/home-page.js.map
- [x] Updated assets/js/iiif-thumbnails/resolve.js
- [x] Updated assets/js/iiif-thumbnails/explicit-thumbnails.js
- [x] Updated assets/js/iiif-thumbnails/home.js
- [x] Updated assets/js/iiif-thumbnails/objects-index.js
- [x] Updated assets/js/iiif-url-warning.js
- [x] Updated assets/js/iiif-url-warning.js.map
- [x] Updated assets/js/iiif-url-warning/main.js
- [x] Updated assets/js/object-page.js
- [x] Updated assets/js/object-page.js.map
- [x] Updated assets/js/object-page/main.js
- [x] Updated assets/js/object-page/image-object.js
- [x] Updated assets/js/object-page/video-object.js
- [x] Updated assets/js/object-page/audio-object.js
- [x] Updated assets/js/object-page/clip-panel.js
- [x] Updated assets/js/object-page/copy-feedback.js
- [x] Updated assets/js/objects-filter.js
- [x] Updated assets/js/objects-filter.js.map
- [x] Updated assets/js/objects-filter/main.js
- [x] Updated assets/js/objects-filter/matching.js
- [x] Updated assets/js/objects-filter/search-index.js
- [x] Updated assets/js/objects-filter/escape.js
- [x] Updated assets/js/objects-index-page.js
- [x] Updated assets/js/objects-index-page.js.map
- [x] Updated assets/js/share-panel.js
- [x] Updated assets/js/share-panel.js.map
- [x] Updated assets/js/share-panel/main.js
- [x] Updated assets/js/share-panel/warnings.js
- [x] Updated assets/js/telar-story.js
- [x] Updated assets/js/telar-story.js.map
- [x] Updated assets/js/telar-story/card-pool.js
- [x] Updated assets/js/telar-story/navigation.js
- [x] Updated scripts/upgrade.py
- [x] Updated scripts/build_local_site.py
- [x] Updated scripts/check_jekyll_conflicts.py
- [x] Updated scripts/encrypt_protected_stories.py
- [x] Updated scripts/generate_collections.py
- [x] Updated scripts/generate_iiif.py
- [x] Updated scripts/iiif_utils.py
- [x] Updated scripts/process_pdf.py
- [x] Updated scripts/telar/build_conflicts.py
- [x] Updated scripts/telar/demo.py
- [x] Updated scripts/telar/story_pages.py
- [x] Updated scripts/telar/widgets.py
- [x] Updated scripts/telar/processors/stories.py
- [x] Updated scripts/telar/processors/objects/__init__.py
- [x] Updated scripts/telar/processors/objects/christmas_tree.py
- [x] Updated scripts/telar/processors/objects/featured.py
- [x] Updated scripts/telar/processors/objects/frame.py
- [x] Updated scripts/telar/processors/objects/local.py
- [x] Updated scripts/telar/processors/objects/remote.py
- [x] Removed assets/js/iiif-thumbnails.js — superseded by the files installed with this upgrade
- [x] Removed scripts/telar/processors/objects.py — superseded by the files installed with this upgrade
- [x] Updated assets/js/README.md
- [x] Updated assets/js/home-page.js
- [x] Updated assets/js/iiif-url-warning.js
- [x] Updated assets/js/katex-loader.js
- [x] Updated assets/js/object-theme.js
- [x] Updated assets/js/story-unlock.js
- [x] Updated assets/js/telar.js
- [x] Updated assets/js/object-audio.js
- [x] Updated assets/js/object-audio.js.map
- [x] Updated assets/js/object-image.js
- [x] Updated assets/js/object-image.js.map
- [x] Updated assets/js/object-video.js
- [x] Updated assets/js/object-video.js.map
- [x] Updated assets/js/object-page/audio-entry.js
- [x] Updated assets/js/object-page/audio-object.js
- [x] Updated assets/js/object-page/boot.js
- [x] Updated assets/js/object-page/clip-panel.js
- [x] Updated assets/js/object-page/image-entry.js
- [x] Updated assets/js/object-page/image-object.js
- [x] Updated assets/js/object-page/video-entry.js
- [x] Updated assets/js/objects-filter.js
- [x] Updated assets/js/objects-filter.js.map
- [x] Updated assets/js/objects-filter/escape.js
- [x] Updated assets/js/objects-filter/main.js
- [x] Updated assets/js/objects-index-page.js
- [x] Updated assets/js/share-panel.js
- [x] Updated assets/js/share-panel.js.map
- [x] Updated assets/js/share-panel/main.js
- [x] Updated assets/js/embed.js
- [x] Updated assets/js/telar-story.js
- [x] Updated assets/js/telar-story.js.map
- [x] Updated assets/js/telar-story/audio-card.js
- [x] Updated assets/js/telar-story/audio-layout.js
- [x] Updated assets/js/telar-story/authoring-frame.js
- [x] Updated assets/js/telar-story/camera-move.js
- [x] Updated assets/js/telar-story/camera-travel.js
- [x] Updated assets/js/telar-story/card-fit.js
- [x] Updated assets/js/telar-story/card-height.js
- [x] Updated assets/js/telar-story/card-pool.js
- [x] Updated assets/js/telar-story/deep-link.js
- [x] Updated assets/js/telar-story/iiif-card.js
- [x] Updated assets/js/telar-story/ios-device.js
- [x] Updated assets/js/telar-story/iiif-manifest.js
- [x] Updated assets/js/telar-story/iiif-viewer.js
- [x] Updated assets/js/telar-story/layout-mode.js
- [x] Updated assets/js/telar-story/main.js
- [x] Updated assets/js/telar-story/media-arrangement.js
- [x] Updated assets/js/telar-story/move-plan.js
- [x] Updated assets/js/telar-story/navigation.js
- [x] Updated assets/js/telar-story/panels.js
- [x] Updated assets/js/telar-story/scroll-engine.js
- [x] Updated assets/js/telar-story/state.js
- [x] Updated assets/js/telar-story/story-input.js
- [x] Updated assets/js/telar-story/utils.js
- [x] Updated assets/js/telar-story/video-card.js
- [x] Updated assets/js/telar-story/video-layout.js
- [x] Updated assets/js/telar-story/viewer.js
- [x] Updated assets/js/telar-story/plates/audio-plate.js
- [x] Updated assets/js/telar-story/plates/base-plate.js
- [x] Updated assets/js/telar-story/plates/framing.js
- [x] Updated assets/js/telar-story/plates/iiif-plate.js
- [x] Updated assets/js/telar-story/plates/media-plate.js
- [x] Updated assets/js/telar-story/plates/video-plate.js
- [x] Updated scripts/dev-only-files.txt
- [x] Updated scripts/encrypt_protected_stories.py
- [x] Updated scripts/fetch_demo_content.py
- [x] Updated scripts/generate_collections.py
- [x] Updated scripts/generate_iiif.py
- [x] Updated scripts/iiif_utils.py
- [x] Updated scripts/process_pdf.py
- [x] Updated scripts/telar/__init__.py
- [x] Updated scripts/telar/answer_budget.py
- [x] Updated scripts/telar/config.py
- [x] Updated scripts/telar/core.py
- [x] Updated scripts/telar/csv_utils.py
- [x] Updated scripts/telar/demo.py
- [x] Updated scripts/telar/dev_only_files.py
- [x] Updated scripts/telar/encryption.py
- [x] Updated scripts/telar/frontmatter.py
- [x] Updated scripts/telar/glossary.py
- [x] Updated scripts/telar/glossary_kinds.py
- [x] Updated scripts/telar/glossary_pages.py
- [x] Updated scripts/telar/images.py
- [x] Updated scripts/telar/latex.py
- [x] Updated scripts/telar/markdown.py
- [x] Updated scripts/telar/pages.py
- [x] Updated scripts/telar/story_pages.py
- [x] Updated scripts/telar/theme_colours.py
- [x] Updated scripts/telar/widgets.py
- [x] Updated scripts/telar/processors/project.py
- [x] Updated scripts/telar/processors/stories.py
- [x] Updated scripts/telar/processors/objects/featured.py
- [x] Updated scripts/telar/processors/objects/frame.py
- [x] Updated scripts/telar/processors/objects/local.py
- [x] Removed assets/js/object-page.js — superseded by the files installed with this upgrade
- [x] Removed assets/js/object-page.js.map — superseded by the files installed with this upgrade
- [x] Removed assets/js/object-page/main.js — superseded by the files installed with this upgrade
- [x] Updated assets/js/telar-story.js
- [x] Updated assets/js/telar-story.js.map
- [x] Updated assets/js/telar-story/deep-link.js
- [x] Updated assets/js/telar-story/iiif-card.js
- [x] Updated assets/js/telar-story/scroll-engine.js
- [x] Updated scripts/telar/config.py
- [x] Updated scripts/telar/glossary.py
- [x] Updated scripts/telar/core.py
- [x] Updated scripts/telar/demo.py
- [x] Updated scripts/telar/processors/objects/remote.py
- [x] Removed scripts/migrations/ — this site runs the upgrade launcher, which downloads a verified copy of the migrations each time it runs.

### Documentation (29 files)

- [x] Updated CHANGELOG.md - Added v0.9.4-beta changelog entry
- [x] Updated README.md - README (v1.1.0 features, bilingual)
- [x] Updated CHANGELOG.md - CHANGELOG (v1.1.0 release notes)
- [x] Updated README.md - README (v1.2.0 features, bilingual)
- [x] Updated CHANGELOG.md - CHANGELOG (v1.2.0 release notes)
- [x] Updated README.md - README (v1.2.1 badges and beta notice, bilingual)
- [x] Updated CHANGELOG.md - CHANGELOG (v1.2.1 release notes)
- [x] Updated README.md — README (v1.3.0 badges and beta notice)
- [x] Updated CHANGELOG.md — CHANGELOG (v1.3.0 release notes)
- [x] Removed stale frontmatter keys from index.md: stories_heading (matched v1.2.1 defaults)
- [x] Skipped homepage welcome update in index.md (user has customised it; hash differs from v1.2.1 default)
- [x] Updated glossary intro in pages/glossary.md (matched v1.2.1 default; replaced with v1.3.0 lang-key template)
- [x] Skipped objects intro update in pages/objects.md (user has customised it; hash differs from v1.2.1 default)
- [x] Skipped about page update in telar-content/texts/pages/about.md (user has customised it; hash differs from v1.2.1 default)
- [x] Updated assets/vendor/README.md
- [x] Updated NOTICE
- [x] Updated README.md
- [x] Updated CHANGELOG.md
- [x] Updated assets/vendor/README.md
- [x] Updated NOTICE
- [x] Updated README.md
- [x] Updated README.md
- [x] Updated CHANGELOG.md
- [x] Updated README.md
- [x] Updated CHANGELOG.md
- [x] index.md has its own text in place of the default line, so it was left as it is. To keep the default content, the line is now `{{ lang.index_page.welcome | default: site.data.languages.en.index_page.welcome | markdownify }}`
- [x] Updated pages/glossary.md: its default content now comes from `{% include glossary-intro.html lang=lang %}`
- [x] Updated README.md
- [x] Updated CHANGELOG.md

### Other (17 files)

- [x] Updated assets/img/background-gris.svg - Weave pattern background
- [x] Added show_sections column to telar-content/spreadsheets/project.csv
- [x] Updated CITATION.cff
- [x] Added .gitattributes — marks the generated story bundle as linguist-generated
- [x] Updated .gitattributes
- [x] Updated .ruby-version
- [x] Updated Gemfile
- [x] Updated Gemfile.lock
- [x] Removed the empty column `object_type` from `objects.csv`; `medium` holds your values.
- [x] Removed `layout`, `permalink` from telar-content/texts/pages/about.md: the build sets a page's layout and address itself
- [x] Wrote `related_terms` in telar-content/texts/glossary/carbon-dating.md as a list, so the page links each related term
- [x] Wrote `related_terms` in telar-content/texts/glossary/knot-typology.md as a list, so the page links each related term
- [x] Wrote `related_terms` in telar-content/texts/glossary/pendant-cord.md as a list, so the page links each related term
- [x] Wrote `related_terms` in telar-content/texts/glossary/primary-cord.md as a list, so the page links each related term
- [x] Wrote `related_terms` in telar-content/texts/glossary/subsidiary-cord.md as a list, so the page links each related term
- [x] Story `story-1`, step 3: the answer is too long for the story card. An answer may have up to 5 paragraphs and 18 lines, counting 53 characters to a line and two lines for each paragraph after the first. This one is over, so the build cuts it. Shorten it to keep its ending.
- [x] The answers were counted in the local copies of your spreadsheets. Your site reads a Google Sheet, and the next build reads it again, so make any change in the sheet itself.

## Manual Steps Required

Please complete these steps:

1. **If you use GitHub Pages:**

No action needed. The updated requirements.txt will be picked up automatically on the next build. If your site has PDF objects, trigger a rebuild to generate their IIIF tiles: go to your repository's Actions tab, select the "Build and Deploy" workflow, and click **Run workflow**.
2. **If you work with your site locally:**

Install the new dependency:

`pip install PyMuPDF`

If your site has PDF objects and their IIIF tiles were not previously generated, regenerate them:

`python3 scripts/generate_iiif.py --base-url YOUR_SITE_URL`

(Replace YOUR_SITE_URL with your site's URL, e.g. https://yourusername.github.io/your-repo)
3. **If you use GitHub Pages:**

Replace your `.github/workflows/build.yml` with the latest version from the Telar repository. The new workflow adds an audio processing step that runs conditionally when audio files are detected. Go to https://github.com/UCSB-AMPLab/telar/blob/main/.github/workflows/build.yml, click "Raw", copy the entire file, and replace the contents of `.github/workflows/build.yml` in your repository. ([guide](https://github.com/UCSB-AMPLab/telar/blob/main/.github/workflows/build.yml))
4. **If you work with your site locally:**

Install JavaScript dependencies:

```
npm install
```

This adds lenis (scroll engine), @vimeo/player (video embeds), esbuild (JS bundler), and vitest (test runner).

**Optional — audio support** (only if your site includes audio objects):

```
brew install ffmpeg audiowaveform      # macOS
sudo apt install ffmpeg audiowaveform  # Ubuntu
```

Sites without audio objects do not need these tools.
5. **New features available after upgrade:**

- **Deep linking**: Your story URLs now update as readers scroll. They can copy and share a URL that points to a specific step, optionally with a panel open. No configuration needed — it works automatically.

- **Title cards**: To add a chapter heading between story steps, leave the object column empty for a step row. The question column becomes the heading text. Title cards work with scroll, keyboard, and button navigation.

- **Collection mode**: To flip your homepage to a collection-first layout, add `collection_mode: true` to `_config.yml` (the upgrade script has already added the flag set to `false`). Objects appear first with large thumbnails; stories appear below with smaller thumbnails.

- **Bibliography styling**: To format references with hanging indent in panel content, wrap them in a `:::bibliography` block in your markdown file.

- **Share panel**: The share panel now includes a "this view" tab that copies the current URL with the reader's exact position. ([guide](https://telar.org/docs))
6. **New features available after upgrade:**

- **Section card table of contents**: To display a navigable TOC on a story's title card, add `show_sections: yes` to the story's row in project.csv (or `mostrar_secciones: si` for Spanish-language sites). The TOC automatically lists every section card in the story, linking to each one. Section cards are steps with an empty object column.

- **Section cards**: Unchanged from v1.1.0 — leave the object column empty for a story step to create a section break. With `show_sections` enabled, these appear as navigable links on the title card.

- **Back to Start button**: Stories now show a "Back to Start" button in the top-left corner once readers scroll past the title card. Clicking it returns to the title card. On the title card itself, the button shows "Back to Home" and links to the homepage.

- **Ordinal numbers removed**: Story cards no longer display auto-generated numbers on the homepage, story pages, or object pages. The homepage placeholder shows the first letter of each story title instead.

- **Deep link fix**: Deep links to layer 2 panels (e.g. `#s3l2`) now correctly open layer 1 underneath, so all parent panels are visible. ([guide](https://telar.org/docs))
7. **Bug fix applied automatically — no action required.**

This patch updates `scripts/fetch_demo_content.py` so it tolerates v-prefixed `telar.version` values in `_config.yml` (for example `version: "v1.2.0"` instead of `version: "1.2.0"`). An earlier version of the Telar Compositor's upgrade flow wrote v-prefixed strings into some sites, which caused the demo content fetcher to silently fail and build sites with no demo content. The fix is in the framework file you just received from this upgrade — no further steps are needed on your end.

If your `_config.yml` has a v-prefixed version string, you may leave it as-is; the script now handles both forms. If you prefer, you can also remove the leading `v` manually under the `telar:` section to keep the file consistent with current Telar conventions. ([guide](https://telar.org/docs))
8. **i18n hygiene update applied — most users need to take no action.**

This release wires up Telar's existing language packs in places that previously hardcoded English (homepage empty states, IIIF URL warning, objects-index error messages, JS thumbnail load fallbacks). It also moves the homepage welcome, glossary intro, objects intro, and about page contents into the language pack so Spanish-speaking site owners with `telar_language: es` get sensible defaults.

The migration changed your user-content files **only when a SHA-256 hash check confirmed the file was byte-for-byte identical to the v1.2.1 default**. If you customised any of those pages (welcome paragraph, about description, glossary or objects intros) — even with whitespace edits — the hash differs and your file is preserved untouched.

A new sister-file convention now localizes the about page: a file named `acerca.md` next to `about.md` in `telar-content/texts/pages/`, carrying frontmatter `localized_for: about.md` and `language: es`, is picked up automatically when `telar_language: es`. For sites with `telar_language: es` whose `about.md` is unchanged from the v1.2.1 default, this migration creates `acerca.md` with the default Spanish content automatically. For sites that customised their `about.md`, the migration skips the create — otherwise the new sister file would shadow your customisation at build time. To add another language, create a sister with `language: <code>` (e.g. `language: fr`). ([guide](https://telar.org/docs))
9. **No action required.** v1.4.0 is a runtime-only upgrade.

Your stories, objects, and configuration keep working without any content changes. The headline improvements:

- **Cross-device IIIF centering fixed** — focal points land correctly across phones, tablets, and desktops, including iPad portrait and landscape phones.
- **Lighter and faster** — Tify (and its Vue dependency) removed; OpenSeadragon is now vendored and loaded locally, so the viewer no longer depends on a CDN.
- **iOS Safari stability** — the URL-bar layout jump is fixed and notch safe-area clearance is added.

One note: the upgrade refreshed the framework language packs (en.yml / es.yml). If you had customised either file, re-apply your changes — the new release adds six `object.viewer.*` keys (pagination labels and error messages for the IIIF viewer) that the updated packs already include. ([guide](https://telar.org/docs))
10. **Recommended — update your GitHub Actions workflow files by hand.** For security, GitHub does not let the automated upgrade modify workflow files, so two v1.5.0 improvements are not applied for you:

- `.github/workflows/upgrade.yml` — the upgrade process is now hardened: it downloads its tooling as a release asset, verifies it against the published checksum, and runs it in isolation. This protects your next upgrade.
- `.github/workflows/build.yml` — the `ruby/setup-ruby` action is now pinned to a specific commit, for supply-chain safety.

To apply them, open each file on GitHub, click "Raw", copy the whole file, and replace the contents of the matching file in your repository:

- https://github.com/UCSB-AMPLab/telar/blob/v1.5.0/.github/workflows/upgrade.yml
- https://github.com/UCSB-AMPLab/telar/blob/v1.5.0/.github/workflows/build.yml

If you skip this, your site keeps building and deploying normally — these changes only harden your workflows. ([guide](https://github.com/UCSB-AMPLab/telar/tree/v1.5.0/.github/workflows))
11. **If you customized the language packs, re-apply your changes.** The upgrade refreshed the framework language packs (`en.yml` / `es.yml`). This release adds the protected-story sharing warnings — the messages shown when a share link or embed code includes the access key — which the updated packs already include. ([guide](https://telar.org/docs))
12. **No action needed.** This is a runtime-only fix.

- **If you use GitHub Pages:** your site picks up the fix automatically the next time it builds.
- **If you work with your site locally:** just rebuild your site to use the updated glossary linking. ([guide](https://telar.org/docs))
13. **No action needed.** This is a display-only fix.

- **If you use GitHub Pages:** your site picks up the fix automatically the next time it builds.
- **If you work with your site locally:** just rebuild your site to use the updated warning messages. ([guide](https://telar.org/docs))
14. **No action needed.** This is a display-only fix.

- **If you use GitHub Pages:** your site picks up the translated chrome strings automatically the next time it builds.
- **If you work with your site locally:** just rebuild your site to use them. ([guide](https://telar.org/docs))
15. **Optional — fully translated page titles.** This release also translates the browser-tab titles of the home, objects, and glossary pages through a new `title_key` field. New sites get it automatically. To enable it on your existing site, add `title_key: navigation.home` to the front matter of `index.md`, `title_key: navigation.objects` to `pages/objects.md`, and `title_key: navigation.glossary` to `pages/glossary.md`. Without this, only those three browser-tab titles stay in English; every other string, including the page headings, already follows your site language. ([guide](https://telar.org/docs))
16. **If you use the Telar Compositor: no action needed.** The Compositor updates your build workflow automatically when it upgrades your site. ([guide](https://telar.org/docs))
17. **If you use GitHub Pages with the "Upgrade Telar" workflow, or work locally:** GitHub does not allow the automated upgrade to change workflow files, so your build workflow is not updated for you. Add the following block to `.github/workflows/build.yml`, just before the `jobs:` line (or recopy the file from the latest template):

```yaml
concurrency:
  group: "pages-${{ github.ref }}"
  cancel-in-progress: true
```

Until you do, your site keeps building and deploying correctly — you may just get an occasional spurious "build failed" email when two builds start at the same time. ([guide](https://telar.org/docs))
18. **Update `.github/workflows/build.yml` by hand (required if you use private stories).** v1.6.0 encrypts private stories in a new build step that GitHub does not allow this upgrade to add for you. Copy the current `build.yml` from the Telar repository over yours (open it on GitHub, use "Copy raw contents", replace the whole file, commit). Until you do, marking any story `private: yes` will fail your build on purpose rather than publish it unprotected. Details: https://telar.org/docs/setup/upgrading/#v160-upgrade-notes ([guide](https://telar.org/docs/setup/upgrading/#v160-upgrade-notes))
19. **If you customized the language packs, re-apply your changes.** The upgrade refreshed the framework language packs (`en.yml` / `es.yml`). This release adds several keys — the private-story unlock messages (empty/incorrect key), the embed banner's site-name fallback, audio-player control labels, and widget/glossary strings, among others — which the updated packs already include. ([guide](https://telar.org/docs))
20. **No action needed.** v1.6.1 only fixes the upgrade tooling itself (a missing registration that made upgrades stop at v1.5.4 and report success, instead of continuing to v1.6.0); it does not change anything in your site. ([guide](https://telar.org/docs))
21. **Update `.github/workflows/upgrade.yml` by hand (recommended, not urgent).** GitHub does not allow this upgrade to change workflow files, so this step is manual: copy the current `upgrade.yml` from the Telar repository over yours (open it on GitHub, use "Copy raw contents", replace the whole file, commit). Your current copy installs only some of the Python packages the upgrade needs; the repository's version installs them all. Not urgent: the upgrade tooling now installs its own dependencies as it runs, so future upgrades keep working even if you leave this for later. ([guide](https://telar.org/docs/setup/upgrading/))
22. **Update `.github/workflows/telar-tests.yml` by hand.** The same restriction applies: GitHub will not let the upgrade modify it for you. Copy the current `telar-tests.yml` from the Telar repository over yours (open it on GitHub, use "Copy raw contents", replace the whole file, commit). The updated workflow stops running Telar's internal framework tests on your site, which ends the emails about failed tests that had nothing to do with your content. ([guide](https://telar.org/docs/setup/upgrading/))
23. **No action needed.** This upgrade removed `.github/dependabot.yml` from your site (or the file was already gone). That file only opened automated dependency-update pull requests, a task the Telar release process now handles instead of each site separately. GitHub's security alerts keep working as before. ([guide](https://telar.org/docs))
24. **Update `.github/workflows/build.yml` by hand (recommended).** GitHub does not let an automated upgrade change workflow files, so you need to do this manually: open the current `build.yml` in the Telar repository on GitHub, choose "Copy raw contents", paste it over your copy, and commit. The new workflow reads the Jekyll build log and stops the build when two files claim the same destination, instead of letting one of them win silently. That matters more than it sounds: on a site with protected stories, the page that silently goes missing can be the one a story's encrypted text lands on. The new workflow also pins current versions of the actions it uses. ([guide](https://telar.org/docs/setup/upgrading/))
25. **Update `.github/workflows/upgrade.yml` by hand (recommended, not urgent).** Same restriction: GitHub will not let the upgrade change this file for you. Open the current `upgrade.yml` in the Telar repository, choose "Copy raw contents", paste it over yours, and commit. The new workflow runs the upgrade engine directly from the verified tooling it downloads. Your current copy keeps working, because that tooling now starts with a launcher that fetches the newest release on its own, so this is housekeeping rather than a requirement. ([guide](https://telar.org/docs/setup/upgrading/))
26. **Update `.github/workflows/telar-tests.yml` by hand (optional).** Same restriction. Only the action versions changed in this release, so your site behaves the same either way. If you want every workflow current, open the current `telar-tests.yml` in the Telar repository, choose "Copy raw contents", paste it over yours, and commit. ([guide](https://telar.org/docs/setup/upgrading/))
27. **If you work on your site locally, two things changed.** Telar now needs Ruby 3.2 or newer, and CI builds with 3.2.11. Install a Ruby of at least 3.2 before your next local build. And `scripts/upgrade.py` is now a launcher rather than the upgrade tool itself: run it and it downloads the newest release's verified upgrade tooling and runs that against your site, so your copy never falls behind again, however long it sits between upgrades. ([guide](https://telar.org/docs/setup/upgrading/))
28. **What changed for your content.** Carousel items can declare `width` and `height`, and the build then skips opening each image to measure it. Search on the objects index now matches whole words as well as the beginnings of words. Objects with a single page copy their coordinates without a page number. And the build now encrypts a protected story whose identifier contains an underscore at the page Jekyll actually produces for it. ([guide](https://telar.org/docs))
29. **Update `.github/workflows/build.yml` by hand (recommended).** GitHub does not let an automated upgrade change workflow files, so you need to do this yourself. Open the current `build.yml` in the Telar repository on GitHub, choose "Copy raw contents", paste it over your copy, and commit. The new workflow checks that the saved copy of your object images still exists before it decides not to rebuild them. GitHub deletes that copy after seven days without use, so until now a site that went quiet for a week could publish a text edit with every image missing, on a run that reported success. It also builds with Node 22, and installs only the tools a build needs. ([guide](https://telar.org/docs/setup/upgrading/))
30. **Update `.github/workflows/upgrade.yml` (optional).** Your current copy keeps working. The new one reads your site's version the same way the upgrade does, so the upgrade issue and the summary always name the same starting version. ([guide](https://telar.org/docs/setup/upgrading/))
31. **`.github/workflows/telar-tests.yml` runs Telar's own tests, not your site's (optional).** You can copy the current version from the Telar repository, or delete it together with `tests/`, `pytest.ini` and `vitest.config.js`: nothing your site builds or publishes uses them. ([guide](https://telar.org/docs/setup/upgrading/))
32. **If you keep your stories in a spreadsheet, check the column that marks a story private.** Telar accepted `privada` and `protegida` but not `privado` or `protegido`, and a story marked with one of the two it did not accept was published unencrypted, with no warning, because the build never recognized it as protected. All four spellings work from this release on. If your sheet used either masculine form, treat those stories as having been public until now and decide what to do about it: the next build will encrypt them, but it cannot undo what was already published. ([guide](https://telar.org/docs/site-features/private-stories/))
33. **If your site reads a Google Sheet, check the upgrade summary for a column to delete.** Telar now stops the build when two columns mean the same thing, such as `medium` and `object_type`. The upgrade fixed your local copy, but the build reads your sheet again, so delete the column the summary names from the sheet itself. ([guide](https://telar.org/docs/your-data/google-sheets/))
34. **What changed for your content.** Each step's answer now has to fit its text card: up to 18 lines and five paragraphs, roughly 150 words in a single paragraph. The build cuts a longer answer, and removes widgets, images, tables, code and footnotes from answers; the upgrade summary lists the answers it will shorten, so you can move that text into a layer panel. A `zoom` below 1 now zooms out, so a step that uses one shows more of the object than before. Spreadsheet cells are read as you typed them: `NA`, `N/A`, `null` and `None` are text, and `007` and `7` are different object IDs. Glossary entries can now take a kind in an optional `kind` column, and the `:::glossary` widget places an entry beside the text as a callout. SVG, HEIC, GIF and BMP images can be objects. ([guide](https://telar.org/docs))
35. **No action needed.** v1.8.1 fixes story navigation and two details of the demo content, and no longer reports some valid IIIF manifests as invalid. The upgrade installs the Telar files that changed; your site's content and settings are left as they are. ([guide](https://telar.org/docs/setup/upgrading/))
36. Your site reads its content from a Google Sheet, and the next build reads the sheet again. Delete the column `object_type` from the tab behind `objects.csv` in the sheet itself, or the build will stop on the same two columns.

## Resources

- [Full Documentation](https://telar.org/docs)
- [CHANGELOG](https://github.com/UCSB-AMPLab/telar/blob/main/CHANGELOG.md)
- [Report Issues](https://github.com/UCSB-AMPLab/telar/issues)
