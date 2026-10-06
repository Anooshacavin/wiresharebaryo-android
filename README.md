<div align="center">

# WIRE SHARE BARYO

### Secure AmneziaWG VPN control for Android

<p>
  <strong>Private networking. Precise app routing. Complete control.</strong>
</p>

[![Android 7.0+](https://img.shields.io/badge/Android-7.0%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://www.android.com/)
[![Release](https://img.shields.io/badge/Release-v1.6.30-2563EB?style=for-the-badge)](DOWNLOAD.md)
[![Build](https://img.shields.io/badge/Build-39-0EA5E9?style=for-the-badge)](RELEASE_NOTES.md)
[![APK only](https://img.shields.io/badge/Distribution-APK%20only-7C3AED?style=for-the-badge&logo=android)](#distribution)

<p>
  <a href="https://github.com/Anooshacavin/wiresharebaryo-android/raw/refs/heads/main/download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk"><strong>Download APK</strong></a>
  · <a href="DOWNLOAD.md">Installation guide</a>
  · <a href="RELEASE_NOTES.md">Release notes</a>
  · <a href="#verify-the-apk">Verify checksum</a>
</p>

</div>

<p align="center">
  <a href="assets/BARYO-VPN-poster.png">
    <img src="assets/BARYO-VPN-poster.png" alt="BARYO VPN promotional poster" width="620">
  </a>
</p>

> **WIRE SHARE BARYO** is authored and maintained by **Baryo**, with a focus on dependable Android VPN control, advanced Per-App routing and privacy-first networking.

## Overview

WIRE SHARE BARYO is an APK-only Android client built around AmneziaWG. It is designed for users who need a clear separation between **full-device protection**, **per-application routing** and **fail-closed privacy controls**.

| At a glance | Details |
|---|---|
| Tunnel engine | AmneziaWG userspace tunnel |
| Routing | Full Tunnel, All Apps, Only Selected, Exclude Selected |
| Privacy | DNS anti-leak, IPv4/IPv6 routing, Kill Switch support |
| Android | Android 7.0+ / API 24 |
| Package | `com.wireshare.baryo` |
| Distribution | Compiled APK only; source is intentionally private |

## Feature highlights

### Advanced Per-App routing

- **All Apps** — send every application through the VPN.
- **Only Selected** — route only the applications you choose.
- **Exclude Selected** — protect everything except selected bypass apps.
- **Global policy** — keep one routing policy synchronized across every profile.
- **Fast filters** — All, Browsers, User Apps and System Apps.
- **Browser presets** — quickly protect or bypass detected browsers.
- **Bulk selection** — select or clear visible applications in one action.

### Security-first tunnel controls

- **Full Tunnel** with IPv4 and IPv6 default routes.
- **DNS anti-leak** using profile DNS with a safe fallback.
- **Kill Switch** support with Android Always-on VPN and lockdown behavior.
- **App Bypass** for applications that must stay outside the tunnel.
- Defensive handling for incomplete or inconsistent profile routes.

## Quick start

1. Download the APK using the button above.
2. Install it on an Android 7.0+ device.
3. Import your WireGuard/AmneziaWG profile.
4. Open **Settings → Per-App** and choose the routing mode.
5. For fail-closed protection, enable **Always-on VPN** and **Block connections without VPN** in Android settings.

> **Recommended first setup:** enable Full Tunnel, keep DNS anti-leak enabled, then select **Protect browsers** if normal web browsing must use the VPN.

## Compatibility

| Requirement | Supported |
|---|---|
| Minimum Android | 7.0 Nougat, API 24 |
| Recommended Android | 8.0 or newer |
| ARM 32-bit | Included |
| ARM 64-bit | Included |
| x86 / x86_64 | Included |

## Download and install

### Direct installation

Use the [installation guide](DOWNLOAD.md) for the supported Android versions and the direct APK link. Android may ask you to allow installation from your file manager or browser.

### ADB installation

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

Linux/macOS:

```bash
sha256sum WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
```

Windows PowerShell:

```powershell
Get-FileHash .\WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk -Algorithm SHA256
```

## Troubleshooting

| Symptom | First check |
|---|---|
| Websites do not open | Set Per-App to **All Apps** or **Protect browsers** |
| Only selected apps connect | Check that the mode is not stuck on **Only Selected** |
| DNS appears outside the tunnel | Enable DNS anti-leak and verify profile DNS |
| Traffic stops after disconnect | Review Android Always-on VPN / lockdown settings |
| One profile behaves differently | Confirm the global Per-App policy is enabled |

When reporting an issue, include the Android version, device model, app build, affected profile count, Per-App mode and whether Full Tunnel/DNS anti-leak are enabled. Never include private keys or server credentials.

## Distribution

This public repository distributes the **compiled APK only**. Android source code, Gradle files, private keys, signing material and build internals are intentionally excluded.

The APK is provided for personal testing and use. Do not upload private configuration files, private keys or server credentials.

## Credits

<div align="center">

**Designed and maintained by Baryo**

WIRE SHARE BARYO · v1.6.30 · Build 39

</div>
