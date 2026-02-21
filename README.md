# Spotify Clone 

A simple front-end Spotify-like music player 

## Overview

This is a static HTML/CSS/JS project that demonstrates a basic music player UI and behavior. The player loads song metadata from per-artist/per-mood `info.json` files inside the `songs/` folder and plays local audio files.

## Features

- Responsive player UI
- Play/pause, next/previous controls
- Song metadata loaded from JSON
- Organized `songs/` folder for moods and artists

## Project Structure

Root files and folders:

- `index.html` — main page
- `css/` — styles (`style.css`, `utility.css`)
- `js/` — JavaScript (`script.js`)
- `img/` — images used by the UI
- `songs/` — folders grouped by mood/artist; each contains an `info.json` describing tracks

Example `songs/` subfolders:

- `songs/Angry_(mood)/info.json`
- `songs/Chill_(mood)/info.json`
- `songs/Dark_(mood)/info.json`

Each `info.json` should list tracks and metadata that `script.js` expects (title, artist, file path, cover image, etc.).

## Running Locally

The simplest way is to open `index.html` directly in your browser. For best behavior (and to avoid browser restrictions on local files), run a local HTTP server.

Using Python 3 (works on Windows, macOS, Linux):

```bash
python -m http.server 8000
```

Then open http://localhost:8000 in your browser.

Or use VS Code Live Server extension: open the workspace and click "Go Live".

## Adding Songs

To add new tracks, create a new folder inside `songs/` (for example `songs/MyArtist/`) and add an `info.json` with the expected metadata and the audio files referenced by that JSON. Follow the format used in existing `info.json` files.

## Development Notes

- The player logic is in `js/script.js`.
- Styles are in `css/style.css` and utility helpers in `css/utility.css`.
- Keep media files under the `songs/` folder to match existing relative paths.

## Contributing

This is a small course project; feel free to open issues or add improvements locally.

## License

Use and modify freely for learning purposes.
