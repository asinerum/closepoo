---
name: youtube-downloader
description: Download YouTube videos with customizable quality and format options
use_cases: Testing skill for downloading video in MP4/WebM format and extracting MP3 audio from video
---

# youtube download

> **PREREQUISITE:** Run `pip install yt-dlp` to activate yt-dlp, and also install `ffmpeg` for merging video/audio files

Download a Youtube video at some URL

## Download YouTube video at <URL>

```bash
yt-dlp -f "bestvideo[ext=mp4]+bestaudio[ext=m4a]/best[ext=mp4]/best" <URL>
```

## Extract audio as mp3 from <URL>

```bash
yt-dlp -x --audio-format mp3 <URL>
```
