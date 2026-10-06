<div align="center">

# WIRE SHARE BARYO

### Secure AmneziaWG VPN control for Android

[![Android](https://img.shields.io/badge/Android-7.0%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://www.android.com/)
[![Release](https://img.shields.io/badge/Release-v1.6.30-3284EB?style=for-the-badge)](DOWNLOAD.md)
[![APK](https://img.shields.io/badge/APK-Binary%20Only-7C5CDE?style=for-the-badge&logo=android)](https://github.com/Anooshacavin/wiresharebaryo-android/raw/refs/heads/main/download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk)
[![License](https://img.shields.io/badge/Source-Not%20Included-F49D39?style=for-the-badge)](#distribution)

**A clean, privacy-focused Android VPN client with powerful Per-App routing.**

[Download APK](https://github.com/Anooshacavin/wiresharebaryo-android/raw/refs/heads/main/download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk) · [Release notes](RELEASE_NOTES.md) · [Installation guide](DOWNLOAD.md) · [Verify checksum](#verify-the-apk)

</div>


> **WIRE SHARE BARYO** is authored and maintained by **Baryo** — focused on dependable Android VPN control, advanced Per-App routing and privacy-first networking.

---

## Dashboard

| Capability | Status | Details |
|---|:---:|---|
| AmneziaWG tunnel | ✅ | Native userspace tunnel engine |
| Full Tunnel | ✅ | IPv4 + IPv6 default routing |
| Per-App routing | ✅ | All, Only Selected, Exclude Selected |
| Global policy | ✅ | One policy across every profile |
| Browser detection | ✅ | Android intent discovery + fallbacks |
| App Bypass | ✅ | Exclude selected apps from the VPN |
| DNS anti-leak | ✅ | Profile DNS + safe fallback |
| Kill Switch | ✅ | Android Lockdown integration |
| Source distribution | 🔒 | APK-only public distribution |

## What makes it different?

### Advanced Per-App control

- **ALL APPS** — route every app through the VPN.
- **ONLY SELECTED** — route only the apps you choose.
- **EXCLUDE SELECTED** — route everything through the VPN except bypassed apps.
- **Global policy** — keep the same routing policy across all profiles.
- **Fast filters** — All, Browsers, User Apps and System apps.
- **Browser presets** — Protect browsers or bypass browsers.
- **Bulk selection** — select or clear all visible apps in one tap.

### Security-first networking

- Full Tunnel adds missing IPv4/IPv6 default routes for incomplete profiles.
- DNS anti-leak uses profile DNS and a safe fallback when the profile has no DNS.
- Kill Switch disables socket-level VPN bypass and integrates with Android Lockdown.
- Android’s **Block connections without VPN** option is supported for fail-closed behavior.

## Compatibility

- **Minimum:** Android 7.0 (Nougat), API 24
- **Recommended:** Android 8.0 or newer
- **CPU:** ARM 32-bit, ARM 64-bit, x86 and x86_64 are included

## Installation

### Direct install

1. Download the APK from [Releases](DOWNLOAD.md).
2. Allow installation from your file manager if Android asks.
3. Install and import your `.conf` profile.
4. Open **Settings → Per-App** to configure routing.

### ADB install

```bash
adb install -r download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
```

## Verify the APK

```text
File: download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
Version: 1.6.30
Build: 39
Package: com.wireshare.baryo
SHA-256: 125989e7cb9c01624ec3bab5af9f294d71a21eff2cd343a99ec67387668861a4
```

Linux/macOS:

```bash
sha256sum download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
```

Windows PowerShell:

```powershell
Get-FileHash .\download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk -Algorithm SHA256
```

## Recommended setup

1. Enable **Full Tunnel**.
2. Keep **DNS anti-leak** enabled.
3. For browser traffic through the VPN, use **Protect browsers**.
4. For browser bypass, use **Bypass browsers**.
5. For a real kill switch, enable Android **Always-on VPN** and **Block connections without VPN**.

## Distribution

This repository intentionally distributes the **compiled APK only**. Android source code, Gradle files, private keys, signing material and build internals are not included.

The APK is distributed for personal testing and use. Do not upload private configuration files, private keys or server credentials to this repository.

## Support checklist

Before reporting a connection issue, include:

- Android version and device model.
- App version/build.
- Whether the issue affects all profiles or one profile.
- Per-App mode in use.
- Whether Full Tunnel and DNS anti-leak are enabled.
- Sanitized Activity/Diagnostics logs without private keys.

<div align="center">

### Built for controlled, private Android networking

**WIRE SHARE BARYO · v1.6.30 · Build 39**

</div>
