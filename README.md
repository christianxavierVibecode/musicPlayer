# HarmonyStream

<p align="center">
  <img src="assets/harmony-stream-preview.svg" alt="HarmonyStream placeholder preview" width="800">
</p>

<p align="center">
  <strong>A browser-based local music player built with HTML, Tailwind CSS, and vanilla JavaScript.</strong>
</p>

<p align="center">
  <a href="https://music-player-gamma-orpin.vercel.app"><strong>Live Demo / Testing Link</strong></a>
</p>

## Overview

HarmonyStream lets users upload and play local audio files directly in the browser. Tracks are kept in an IndexedDB library, so they remain available after refreshing the page. No account or backend server is required.

## Features

- Upload one or more local audio files
- Persistent music library powered by IndexedDB
- Play, pause, previous, next, shuffle, and repeat controls
- Seekable progress timeline
- Volume controls and keyboard shortcuts
- Audio frequency visualization with the Web Audio API
- Equalizer presets:
  - Flat
  - Bass Boost
  - Pop
  - Rock
  - FxSound Super Bass
- Add and remove individual tracks or clear the full library
- Responsive Tailwind CSS interface

## Technology Stack

- HTML5
- Vanilla JavaScript
- Tailwind CSS
- HTML5 Audio API
- Web Audio API
- IndexedDB
- Font Awesome

## Getting Started

HarmonyStream is a static web application and can be served from any local web server.

### Run locally

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080` in a modern browser.

> You can also open `index.html` directly, but a local server is recommended for consistent browser behavior.

## Usage

1. Select **Add Music** and choose one or more audio files.
2. Select a track from **Your Library** to play it.
3. Use the player controls to seek, adjust volume, shuffle, repeat, or change the equalizer preset.
4. Use the three-dot menu beside a track to remove it.
5. Use the trash button to clear the complete library.

## Keyboard Shortcuts

| Action | Shortcut |
|---|---|
| Play / pause | `Space` |
| Rewind / forward 5 seconds | `←` / `→` |
| Increase / decrease volume | `↑` / `↓` |
| Delete the current track | `Delete` or `Ctrl + Delete` |
| Open file upload / clear library | `Ctrl + Enter` |
| Open / close shortcut help | `Ctrl + /` |
| Close shortcut help | `Esc` |

## Deployment

The project is deployed on Vercel:

- **Testing / live demo:** https://music-player-gamma-orpin.vercel.app

Because this is a static application, it can also be deployed to GitHub Pages or any static hosting provider.

## Project Structure

```text
.
├── index.html       # Application markup, styling, and JavaScript
├── tailwind.js      # Tailwind CSS browser build
├── logo.png         # Application icon
└── assets/
    └── harmony-stream-preview.svg
```

## Browser Notes

- Audio and equalizer behavior requires a modern browser with Web Audio API support.
- Uploaded files are stored in IndexedDB; clearing browser site data will clear the library.
- Supported formats depend on the audio formats available in the browser.

## License

No license has been specified for this repository.
