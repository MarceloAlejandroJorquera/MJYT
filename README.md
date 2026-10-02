# MJYT

MJYT is a native Windows x64 YouTube downloader focused on a compact, responsive desktop UI, high-throughput downloads, retained queue workflows, and a portable single-executable runtime.

> **Repository scope:** this public repository contains MJYT documentation, release notes, screenshots, and release metadata only. **MJYT application source code is not published here.** GitHub's automatically generated **Source code (zip/tar.gz)** downloads contain only this documentation repository; they are not the application's source code.

## Highlights

- Download individual YouTube videos and playlists.
- Choose download format, audio language/track policy, and subtitle policy.
- Download adaptive media streams and supported live streams.
- Embed metadata, cover artwork, and selected subtitles when supported by the destination container.
- Queue multiple links, retain queue state, reorder pending work, retry items, and pause/resume supported transfers.
- Show video thumbnails directly in the queue.
- Configure default format/audio/subtitle behavior, destination, paste behavior, and download speed limits.
- Run a built-in throughput benchmark and review benchmark reports in the UI.
- Native dark Windows interface with a portable application icon and no installer requirement.
- No downloader, JavaScript engine, FFmpeg, or other helper executable is required beside the released MJYT executable at runtime.

## Download

Official Windows x64 binaries are distributed from the repository's **Releases** page.

For normal use, download:

```text
MJYT-v1-windows-x64.zip
```

Extract it and run:

```text
MJYTv1.exe
```

The standalone `MJYTv1.exe` may also be attached directly to the release.

MJYT is portable and does not require installation.

## Quick start

1. Run `MJYTv1.exe`.
2. Add one or more supported YouTube links.
3. Analyze the rows if needed, then choose format/audio/subtitle options.
4. Select the destination and optional speed limit.
5. Start or resume the queue.
6. Completed media is written to the selected destination.

See [Usage](docs/USAGE.md) for a more complete walkthrough.

## Screenshots

Public screenshots may be added under [`docs/images/`](docs/images/) after checking them for private paths, account information, or other local-only details.

## Platform

- Windows 10/11 x64
- 64-bit release only

## Update checks

MJYT includes an optional **Check new versions** setting. When enabled, it performs an asynchronous lookup of the latest MJYT GitHub release after startup and periodically while the application remains open. It does not automatically download or execute an update.

See [Network & privacy](docs/NETWORK_AND_PRIVACY.md) for the public network-behavior summary.

## Current limitations

- MJYT is intended for YouTube URLs; it is not a general multi-site downloader.
- Private, members-only, account-authenticated, rented/purchased, and DRM-protected media are not supported in v1.
- Media availability still depends on what YouTube exposes to the application and on YouTube's current delivery behavior.
- YouTube can change its web/player interfaces; such changes can require an MJYT update.

See [FAQ](docs/FAQ.md) for common questions.

## Release integrity

Official binary releases include SHA-256 checksums. Verify downloaded artifacts against `SHA256SUMS.txt` from the same GitHub Release.

See [Release integrity](docs/RELEASE_INTEGRITY.md).

## Versioning

MJYT uses lineage-style release labels rather than Semantic Versioning. The sequence begins with `v1`, followed by `v1.1`, `v1.1.1`, `v1.1.1.1`, and so on.

See [Versioning](docs/VERSIONING.md).

## Licensing

MJYT itself is **not open source** and no public redistribution license has been granted for the MJYT application binaries or proprietary project materials. See [LICENSE.txt](LICENSE.txt).

Third-party assets retain their own licenses. See [Third-party notices](docs/THIRD_PARTY.md).

## Support

For usage problems, bug reports, or feature requests, see [SUPPORT.md](SUPPORT.md).

## Disclaimer

MJYT is not affiliated with or endorsed by YouTube or Google. Users are responsible for complying with applicable laws, copyright requirements, and service terms when downloading media.
