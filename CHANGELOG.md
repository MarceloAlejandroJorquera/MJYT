# Changelog

## v1.1 — 2026-10-19

Public playlist and streamed-video compatibility release.

### Fixed

- Public completed livestream and active-stream routing, including native DASH/HLS handling where supported.
- Standard public playlist enumeration and pagination across supported YouTube response formats.
- Generated radio Mix traversal and continuation handling.
- YouTube Music-generated public compilation playlists (`RDCLAK...`), including modern `lockupViewModel` entries and continuation discovery.
- Avoided importing unrelated sidebar recommendations when resolving public playlist inventory.
- Improved playlist routing diagnostics while excluding private, members-only, account-authenticated, and DRM-protected items.

### Release

- Release identity `v1.1`, title `MJYT v1.1`, and Windows resource FileVersion/ProductVersion `1.1`.
- Portable executable renamed `MJYTv1.1.exe`; GitHub release provides a ZIP containing the executable and its checksum.

## v1 — 2026-10-01

First public binary and source release of MJYT.

### Added

- Native Windows x64 YouTube extraction and download pipeline.
- Portable single-executable runtime with the application font and icon embedded into `MJYTv1.exe`.
- Video, audio, playlist, adaptive-stream, subtitle, metadata, cover-art, and supported live-stream handling.
- Queue persistence, retry/reorder controls, pause/resume support, destination management, and bandwidth limiting.
- Queue thumbnails and retained virtualized list rendering.
- User-selectable format, audio/language, subtitle, and destination defaults.
- Built-in selected-download benchmark and user-facing benchmark results.
- Native dark UI with custom title bar, responsive queue, virtual console, Options dialog, Add Links dialog, and Windows taskbar/shortcut icon integration.
- Optional persisted GitHub release checks: first lookup about 10 seconds after startup, periodic checks about every 6 hours, and a compact in-app new-version notification linking to the matching release page.
- Full Release qualification covering the native extraction, transfer, media-finalization, portability, and regression gates before release packaging.
- Public repository/readme screenshot set covering the main window, Add Links dialog, benchmark, report, and Options views.

### Release notes

- Windows 10/11 x64 only.
- No runtime helper executables are required.
- Account-authenticated/private/members-only and DRM-protected media are not supported.
