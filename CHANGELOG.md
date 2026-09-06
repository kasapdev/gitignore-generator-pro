# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [1.0.1] - 2026-09-06

### Fixed

- The global `mod+C` keyboard shortcut no longer hijacks the browser's native copy-selection behavior. Previously, pressing Ctrl/Cmd+C always called `preventDefault()` and copied the *entire* merged `.gitignore` output, even if the user had manually selected a smaller snippet of text on the page (e.g. inside the preview pane) intending a normal copy of just that selection. The shortcut handler in `assets/js/core.js` now checks for an active text selection before intercepting `mod+C`, and defers to the browser's native copy when one exists.
- Corrected the stale `<meta name="description">` in `index.html`, which advertised "18+ curated stack templates" while the app (and README) actually ships 26.
