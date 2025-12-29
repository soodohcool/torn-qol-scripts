# Changelog

All notable changes to the Christmas Town Helper script will be documented in this file.

## [3.0.8] - 2025-12-19 — Antonon_Balloni[3853029]

### Added
- **Combo Chest Cracker**: New helper UI that assists with cracking combination chests
  - Displays only when you pick up and open a combo chest (not just when one is visible on the map)
  - Tracks your attempts with color-coded feedback (red/yellow/green)
  - Filters possible combinations (729 total) based on feedback
  - Shows suggested combinations to try next
  - Automatically closes when you close the combo chest UI
  - Can be enabled/disabled in settings like other game helpers (Hangman, Word Fixer, etc.)
  - Added "Combo Cracker Helper" option to the settings menu (defaults to enabled)

- **AFK Mode**: Track items collected from mystery gifts while away
  - Toggle button in the header (red = off, green = on)
  - Automatically tracks all items collected from mystery gifts
  - Shows a summary modal with item names, quantities, and values when disabled
  - Dark mode support

- **Background Audio Playback**: Chirp alerts now play even when the browser tab is in the background
  - Uses Web Audio API for reliable background playback
  - Falls back to standard audio if Web Audio is unavailable
  - Automatically enables on first user interaction (browser requirement)

### Changed
- Optimized game helper UI updates to prevent page shake when moving on the map
- Improved combo chest detection using URL, request body, and response data

### Fixed
- Combo chest helper no longer interferes with other game helpers (Hangman, Word Fixer, etc.)

### Removed
- Debug console.log statements for cleaner console output

