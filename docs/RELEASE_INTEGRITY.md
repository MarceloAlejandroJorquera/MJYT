# Release integrity

Official MJYT binary releases provide SHA-256 checksums in `SHA256SUMS.txt`.

## Verify with PowerShell

From the directory containing the downloaded file:

```powershell
Get-FileHash .\MJYTv1.exe -Algorithm SHA256
```

or, for the portable archive:

```powershell
Get-FileHash .\MJYT-v1-windows-x64.zip -Algorithm SHA256
```

Compare the resulting hexadecimal SHA-256 value with the matching filename in `SHA256SUMS.txt` from the **same GitHub Release**.

A matching SHA-256 establishes that the downloaded bytes are identical to the bytes represented by that checksum. It does not replace normal operating-system security controls or user judgment about where a file was obtained.

## Expected v1 binary assets

The binary release page is expected to provide:

```text
MJYTv1.exe
MJYT-v1-windows-x64.zip
SHA256SUMS.txt
```

The project does not publish an MJYT application-source archive as a v1 release asset.
