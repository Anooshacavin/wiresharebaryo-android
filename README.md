# WIRE SHARE BARYO

## Secure AmneziaWG VPN Control for Android

[![Android 7.0+](https://img.shields.io/badge/Android-7.0%2B-22C55E?style=for-the-badge&logo=android&logoColor=white)](https://www.android.com/)
[![Release v1.6.30](https://img.shields.io/badge/Release-v1.6.30-2563EB?style=for-the-badge)](RELEASE_NOTES.md)
[![Build 39](https://img.shields.io/badge/Build-39-7C3AED?style=for-the-badge)](RELEASE_NOTES.md)
[![APK Only](https://img.shields.io/badge/Distribution-APK%20Only-F97316?style=for-the-badge&logo=android&logoColor=white)](#distribution)

> **Private networking. Precise app routing. Complete control.**
>
> Authored and maintained by **Baryo**.

![BARYO VPN promotional poster](assets/BARYO-VPN-poster.png)

---

## Download the APK

### Click the green button below to download and install the app

[![Download APK](https://img.shields.io/badge/DOWNLOAD%20APK-DIRECT-16A34A?style=for-the-badge&logo=android&logoColor=white)](https://github.com/Anooshacavin/wiresharebaryo-android/raw/refs/heads/main/download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk)

You do **not** need to open the **Code** menu or download the repository files. Use the green **DOWNLOAD APK** button above.

- [Installation guide](DOWNLOAD.md)
- [Release notes](RELEASE_NOTES.md)
- [Direct APK file](download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk)

---

## Overview

WIRE SHARE BARYO is an APK-only Android client built around the AmneziaWG userspace tunnel. It provides full-device VPN protection, advanced Per-App routing and privacy-focused connection controls.

| Item | Details |
|---|---|
| Tunnel | AmneziaWG userspace tunnel |
| Package | `com.wireshare.baryo` |
| Version | `1.6.30` |
| Build | `39` |
| Minimum Android | Android 7.0 / API 24 |
| Distribution | Compiled APK only |

## Key features

### Per-App routing

- **All Apps** — route every installed app through the VPN.
- **Only Selected** — route only the apps you choose.
- **Exclude Selected** — route everything through the VPN except bypassed apps.
- **Global policy** — keep one routing policy across every profile.
- **Browser filter** — quickly find and manage installed browsers.
- **User and system filters** — separate ordinary apps from system apps.
- **Bulk selection** — select or clear multiple apps efficiently.

### Security controls

- **Full Tunnel** with IPv4 and IPv6 default routes.
- **DNS anti-leak** using profile DNS with a safe fallback.
- **Kill Switch** support through Android Always-on VPN and lockdown settings.
- **App Bypass** for apps that must stay outside the tunnel.
- Defensive handling for incomplete profile routes.

## Quick start

1. Click **Download APK** above.
2. Install the APK on an Android 7.0+ device.
3. Import your WireGuard or AmneziaWG profile.
4. Open **Settings → Per-App**.
5. Choose **All Apps**, **Only Selected** or **Exclude Selected**.
6. For fail-closed protection, enable **Always-on VPN** and **Block connections without VPN** in Android settings.

### Recommended setup

1. Enable **Full Tunnel**.
2. Keep **DNS anti-leak** enabled.
3. Use **All Apps** when normal web browsing must use the VPN.
4. Use **Only Selected** when you want a strict app allowlist.
5. Use **Exclude Selected** when only a few apps should bypass the VPN.

## Compatibility

| Platform | Support |
|---|---|
| Android 7.0 Nougat / API 24 | Supported |
| Android 8.0 and newer | Recommended |
| ARM 32-bit | Included |
| ARM 64-bit | Included |
| x86 / x86_64 | Included |

## Installation

### Android

1. Download the APK from the green button above.
2. Allow installation from your browser or file manager if Android asks.
3. Install the application.
4. Import your VPN profile.

### ADB

```bash
adb install -r WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
```

## Verify the APK

```text
File: WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
Version: 1.6.30
Build: 39
Package: com.wireshare.baryo
SHA-256: 125989e7cb9c01624ec3bab5af9f294d71a21eff2cd343a99ec67387668861a4
```

### Linux and macOS

```bash
sha256sum WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
```

### Windows PowerShell

```powershell
Get-FileHash .\WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk -Algorithm SHA256
```

## Troubleshooting

| Problem | What to check |
|---|---|
| Websites do not open | Use **All Apps** or verify that your browser is included in **Only Selected**. |
| Only a few apps connect | Check whether Per-App is set to **Only Selected**. |
| DNS appears outside the tunnel | Enable **DNS anti-leak** and verify the profile DNS. |
| Traffic stops after disconnect | Review Android Always-on VPN and lockdown settings. |
| One profile behaves differently | Confirm that the global Per-App policy is enabled. |

When reporting an issue, include your Android version, device model, app version, build number and Per-App mode. Do not upload private keys, server credentials or unsanitized VPN configurations.

## Distribution

This public repository distributes the **compiled APK only**. Android source code, Gradle files, private keys, signing material and build internals are intentionally excluded.

The APK is provided for personal testing and use. Do not upload private configuration files or credentials.

---

**WIRE SHARE BARYO** · v1.6.30 · Build 39  
Designed and maintained by **Baryo**.
