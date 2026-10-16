# Trustity Linux Releases

Official ISO images for Trustity Linux.

## Beta 1.0.5 (amd64)

GitHub limits release files to 2 GB, so the ISO is split into three parts. Download all parts from the [1.0.5-beta release](https://github.com/Trustity/trustity-linux-releases/releases/tag/v1.0.5-beta) and join them:

**macOS / Linux**
```
cat trustity-linux-desktop-amd64.hybrid.iso.part-0{0,1,2} > trustity-linux-1.0.5-beta-amd64.iso
shasum -a 256 trustity-linux-1.0.5-beta-amd64.iso
```

**Windows**
```
copy /b trustity-linux-desktop-amd64.hybrid.iso.part-00+trustity-linux-desktop-amd64.hybrid.iso.part-01+trustity-linux-desktop-amd64.hybrid.iso.part-02 trustity-linux-1.0.5-beta-amd64.iso
certutil -hashfile trustity-linux-1.0.5-beta-amd64.iso SHA256
```

SHA-256: `dcbf947f9e378971cbc23e296eab5bf1616189c2c6e38a0089727c38d0f2091b`
