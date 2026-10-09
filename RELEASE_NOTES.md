# WIRE SHARE BARYO v1.6.38 — Build 47

## Advanced UI and network tuning release

### New

- **Smart Speed Boost** is enabled by default and applies adaptive MTU/network transport tuning in the Android VPN builder.
- **Manual MTU** has colored quick presets, saved-value status, custom validation and safe-range feedback.
- Three selectable visual themes: **Cloud Studio**, **Ocean Breeze** and **Violet Aurora**.
- About page updated with current release data, privacy notes and the complete capability summary.

### Improvements

- Existing tunnel, parser, profile storage, Per-App routing, backup/restore and diagnostics behavior preserved.
- APK package remains `com.wireshare.baryo` so compatible local installations can update in place.
- Release is distributed as APK-only; Android source, Gradle files and private signing material are intentionally not published here.

## Install

[Download the official APK](https://github.com/Anooshacavin/wiresharebaryo-android/releases/tag/v1.6.38)

```bash
adb install -r WIRESHAREBARYO-1.6.38-build47.apk
```

## Verification

- Version: `1.6.38`
- Build: `47`
- SHA-256: `abdcba22cf18c2eb44f6d0ff38a989f0a4014a24c4e1c431d1eab8a466205b1b`
- Unit tests: 20 passed, 0 failed
- APK signature: verified with APK Signature Scheme v2
