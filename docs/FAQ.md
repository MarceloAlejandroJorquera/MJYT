# FAQ

## Is MJYT open source?

No. The public GitHub repository contains documentation, screenshots, release notes, and release metadata. The MJYT application source code is not published there.

## Why does GitHub show "Source code (zip)" and "Source code (tar.gz)" on a release?

GitHub automatically generates those archives from the repository at the release tag. For MJYT, that repository is documentation-only, so those archives contain the public documentation snapshot—not the application's C++ source code.

## Does MJYT require installation?

No. MJYT is distributed as a portable Windows x64 executable/package.

## Does MJYT require yt-dlp, FFmpeg, or a JavaScript runtime beside the executable?

No. The published v1 runtime does not require a downloader helper, external JavaScript engine, FFmpeg executable, or other media-helper executable beside `MJYTv1.exe`.

## Can MJYT download playlists?

Yes, for supported public YouTube playlists. Playlist slicing can use 1-based inclusive `From`/`To` positions.

## Can MJYT download private or members-only videos?

No. MJYT v1 does not support account-authenticated, private, members-only, rented/purchased, or DRM-protected media.

## Does MJYT install a browser extension or system service?

No. MJYT is a portable desktop application.

## Does MJYT automatically update itself?

No. The optional version check can notify you that a newer GitHub release exists and open the release page, but it does not automatically download or execute an update.

## How do I verify the release?

Compare the SHA-256 hash of the downloaded release asset with the matching entry in `SHA256SUMS.txt` from the same GitHub Release. See [Release integrity](RELEASE_INTEGRITY.md).

## Why might a previously working video stop working?

YouTube can change its player, extraction, or media-delivery interfaces. A YouTube-side change can require an MJYT update even when the local application has not changed.
