# Day 23 — Multimedia (audio, video, iframe)

## What I learned
- How to embed a YouTube video using an `<iframe>` (privacy-enhanced `youtube-nocookie`).
- How to use the native `<video>` element with multiple sources and a poster image.
- How to add `<audio>` players for local files and streamed audio.
- Accessibility notes: captions (`<track>`), descriptive titles, and fallback text.

## Files
- `index.html` — demo page with examples.
- `videos/sample.mp4`, `videos/poster.jpg` — demo video + poster.
- `audio/song.mp3`, `audio/song.ogg` — demo audio files.
- `captions/en.vtt` — sample captions file for the video.

## Run locally
1. Clone repo.
2. Serve the folder (recommended: live server or `python -m http.server 8000`).
3. Open `http://localhost:8000/` and test the players.

## Notes
- Use multiple source formats (MP4 / WebM for video; MP3 / OGG for audio) to maximize browser compatibility.
- For captions use WebVTT (`.vtt`) files and include them via `<track kind="captions">`.
- For YouTube embeds you can use query params to control autoplay, controls, start time, etc. Use `youtube-nocookie` for reduced tracking.
