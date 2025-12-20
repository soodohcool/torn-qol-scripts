# Changelog

All notable changes to the Christmas Town Helper script will be documented in this file.

## [3.0.8] - 2025-12-19 — Antonon_Balloni[3853029]

### Added
- **Combo Chest Cracker**: New helper UI that assists with cracking combination chests
  - Displays when a combination chest is detected on the map
  - Tracks your attempts with color-coded feedback (red/yellow/green)
  - Filters possible combinations (729 total) based on feedback
  - Shows suggested combinations to try next
  - Persists during map movement - doesn't close when you move around

- **Background Audio Playback**: Chirp alerts now play even when the browser tab is in the background
  - Uses Web Audio API for reliable background playback
  - Falls back to standard audio if Web Audio is unavailable
  - Automatically enables on first user interaction (browser requirement)

### Changed
- Optimized game helper UI updates to prevent page shake when moving on the map
- Improved combo chest detection using URL, request body, and response data

### Removed
- Debug console.log statements for cleaner console output

