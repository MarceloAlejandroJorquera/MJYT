# MJYT v1

MJYT v1 is the first public binary release of the native Windows x64 YouTube downloader.

## Highlights

- Portable `MJYTv1.exe` with no installer required.
- Native video and playlist extraction/download pipeline.
- Video format and audio-language/track selection.
- Explicit subtitle selection with native container embedding when supported.
- Native metadata and cover-art embedding when supported.
- Queue thumbnails, persistent queue state, retry/reorder controls, pause/resume behavior, download history, and destination management.
- Adaptive-stream and supported live-stream handling.
- Configurable download speed limit.
- Built-in throughput benchmark with user-facing report views.
- Custom dark Windows UI with embedded MJYT icon and Anonymous Pro interface font.
- Optional **Check new versions** setting with asynchronous GitHub release checks.
- No external downloader, JavaScript engine, FFmpeg, or other helper executable is required beside the released executable at runtime.

## Release assets

The normal portable package is:

```text
MJYT-v1-windows-x64.zip
```

The standalone executable may also be attached directly as:

```text
MJYTv1.exe
```

Verify release assets with:

```text
SHA256SUMS.txt
```

The public GitHub repository does **not** contain the MJYT application source code. GitHub-generated "Source code" archives correspond only to the documentation repository snapshot.

## Requirements

- Windows 10/11 x64
- Network access to the requested YouTube media

## Limitations

MJYT v1 does not support private, members-only, account-authenticated, rented/purchased, or DRM-protected media. MJYT is intended for YouTube URLs and may require updates if YouTube changes its web/player or media-delivery interfaces.

## Update checks

When **Check new versions** is enabled, MJYT can query the latest public MJYT release on GitHub and show an in-app notification when a newer lineage release is available. It never automatically installs an update.

## Legal

MJYT is not affiliated with or endorsed by YouTube or Google. Users are responsible for complying with applicable laws, copyright requirements, and service terms.
