# Changelog

## v1 — 2026-10-01

First public **binary** release of MJYT.

### Added

- Native Windows x64 YouTube extraction and download pipeline.
- Portable single-executable distribution as `MJYTv1.exe`.
- Individual-video and playlist workflows.
- Adaptive-stream and supported live-stream handling.
- Format selection, audio-language/track handling, subtitle selection, metadata embedding, and cover-art embedding.
- Persistent retained queue with progress, speed, state, destination, retry/reorder controls, pause/resume behavior, and completed history.
- Queue thumbnails and responsive table-first UI.
- Configurable default format/audio/subtitle behavior, destination, paste behavior, and download speed limits.
- Built-in throughput benchmark and benchmark-report viewer.
- Native dark Win32 interface, custom title bar, Options dialog, Add Links dialog, and embedded application icon/font resources.
- Optional GitHub release checks with an in-app new-version notification.
- Full release qualification covering native extraction, transfer, media finalization, regression, and portability gates before binary staging.

### Runtime model

- No downloader helper executable is required at runtime.
- No external JavaScript runtime is required at runtime.
- No FFmpeg executable or other media-helper executable is required at runtime.

### Supported platform

- Windows 10/11 x64.

### Known limitations

- Private, members-only, account-authenticated, rented/purchased, and DRM-protected media are not supported in v1.
- YouTube-side interface changes can require an MJYT update.

### Repository publication

- The public repository contains documentation, screenshots, release notes, and release metadata only.
- MJYT application source code is not published in this repository.
