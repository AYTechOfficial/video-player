# Playlist Speed Player

A minimal embed-layer website for playing a YouTube playlist with:

- Custom **playback speed control** (0.25×–2×, persists across videos and sessions)
- **Auto-advance**: the next video starts automatically when the current one ends
- Playlist sidebar with titles, click-to-jump, current-video highlight
- Prev/Next, loop playlist and autoplay-next toggles
- Paste any playlist URL or ID in the header to load a different playlist (defaults to `PLMA7XybhrXew`)

Single static file (`index.html`) — built on the YouTube IFrame Player API + YouTube oEmbed.

## Deploy (GitHub Pages)

1. Push `index.html` to the root of a repository.
2. Settings → Pages → Source: `main` branch, `/ (root)`.

## Local dev

```bash
python3 -m http.server 8765
# open http://127.0.0.1:8765
```

Note: playback start requires a user click (browser autoplay policy).
