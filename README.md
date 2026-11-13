# AusSight outbox
Packages for the AusSight posting bot. Up to two stories a day, plus on-demand requests.

- `latest/index.json` — today's packages: one entry per slot with status, headline and URLs.
- `latest/package-1.json`, `latest/package-2.json` — today's two stories (each with its own `video-N.mp4`, `captions-N.srt`, `cover-N.png` and `cover-vertical-N.png`).
- Videos: `video_url` (1080×1350, for X and LinkedIn) and `video_vertical_url` (1080×1920, the same video with the picture filling the screen, for Instagram Reels, YouTube Shorts and TikTok).
- Covers: `cover_url` (1080×1350, the same image the video opens on) and `cover_vertical_url` (1080×1920, Instagram Reels cover). Set them as the video's cover/thumbnail on every platform that takes one; a text-only package has covers too, attached to its posts as the image.
- `latest/package-request.json` — the latest on-demand package.
- `latest/package.json` — story 1 (or the latest on-demand package), kept for compatibility.

A package with `"status": "no-story"` means nothing qualified for that slot: do not post it.
Generated automatically by AusSight Studio. Do not edit by hand.
