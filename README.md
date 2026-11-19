# Merge and Extract

Download all 80 archive parts (`video_pool.zip.001` through `video_pool.zip.080`) and `SHA256SUMS` into the same directory, then verify the checksums, merge the parts, and extract the archive:

```bash
sha256sum -c SHA256SUMS
cat video_pool.zip.[0-9][0-9][0-9] > video_pool.zip
unzip video_pool.zip
```

On macOS, replace the first command with `shasum -a 256 -c SHA256SUMS`.
