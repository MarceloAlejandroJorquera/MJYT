# Using MJYT v1

## 1. Start MJYT

Run `MJYTv1.exe`. MJYT is portable and does not require installation.

## 2. Add links

Use the Add Links workflow or paste supported YouTube URLs into MJYT. Multiple links can be added in one operation.

Supported public workflows include ordinary video URLs and playlist URLs. MJYT v1 is not a general multi-site downloader.

## 3. Analyze queue rows

Analysis resolves the available native media choices for a row and populates the row's relevant format, audio, and subtitle choices.

Queue rows retain their own selected policy/options so later changes to defaults do not silently rewrite already queued work.

## 4. Choose format, audio, and subtitles

MJYT exposes format policies and, when available, exact media choices. Audio-language handling can prefer the original/default audio or a selected language when that choice is available for the media.

Subtitle selection is explicit. Available subtitle tracks can be selected for native embedding when the destination container supports the selected media/subtitle combination.

## 5. Metadata and cover artwork

MJYT can embed supported metadata and cover artwork into the final media container. These are container-level operations; MJYT does not need to leave a separate thumbnail sidecar file beside the completed media.

## 6. Playlists

Playlist expansion is supported for public playlist URLs. Range slicing uses 1-based inclusive positions:

- `From` selects the first playlist item to include.
- `To` selects the last item to include.
- A blank `To` means through the end of the playlist.
- An overlong `To` clamps to the playlist end.

Duplicate expanded URLs are suppressed while preserving first-occurrence order.

## 7. Queue behavior

The retained queue stores pending/completed state across application restarts.

Supported queue actions include:

- Reordering future work.
- Retrying failed/skipped items.
- Skipping the active item.
- Pausing/resuming supported transfers.
- Clearing completed history.

Interrupted active rows return to a pending state after restart so supported transfer state can be resumed.

## 8. Destination and defaults

The Options dialog provides defaults for:

- Format.
- Audio.
- Subtitles.
- Destination.
- Speed limit.
- Immediate analyze/download behavior when links are pasted.

Changing defaults affects new work; existing retained queue rows preserve their already selected row options.

## 9. Speed limit

The Options dialog exposes a download speed limit in MB/s. A zero/unlimited setting leaves MJYT's transfer engine free to use available throughput; a nonzero limit constrains active download traffic to the configured ceiling.

## 10. Benchmark

The built-in benchmark can evaluate MJYT's download path and present a benchmark report in the UI. Benchmark results are environmental: network path, CDN edge, storage performance, and congestion can materially affect measured throughput.

## 11. Update checks

When **Check new versions** is enabled, MJYT can query the latest GitHub release and show a notification when a newer lineage release is published. MJYT does not automatically install the release.

## Unsupported workflows in v1

MJYT v1 does not support:

- Account login or cookie import.
- Private media.
- Members-only media.
- Rented/purchased media.
- DRM-protected media.
