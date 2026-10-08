<div align="center">

# WIRE SHARE BARYO

### Secure AmneziaWG VPN Control for Android

**Private networking · Precise app routing · Complete control**

[![Android 7.0+](https://img.shields.io/badge/Android-7.0%2B-34A853?style=for-the-badge&logo=android&logoColor=white)](https://www.android.com/)
[![Release](https://img.shields.io/badge/Release-v1.6.30-1976D2?style=for-the-badge)](./RELEASE_NOTES.md)
[![Build](https://img.shields.io/badge/Build-39-6C63FF?style=for-the-badge)](./DOWNLOAD.md)
[![APK Only](https://img.shields.io/badge/Distribution-APK%20Only-F97316?style=for-the-badge&logo=android&logoColor=white)](#distribution)

**Authored and maintained by Baryo.**

[![Download APK](https://img.shields.io/badge/⬇%20DOWNLOAD%20APK-16A34A?style=for-the-badge&logo=android&logoColor=white)](https://github.com/Anooshacavin/wiresharebaryo-android/raw/main/download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk)

[Installation](#installation) · [Features](#features) · [Security](#security) · [Privacy](#privacy-and-data-collection) · [Report a bug](https://github.com/Anooshacavin/wiresharebaryo-android/issues/new)

</div>

<p align="center">
  <a href="https://github.com/Anooshacavin/wiresharebaryo-android/blob/main/assets/BARYO-VPN-poster.png">
    <img src="https://github.com/Anooshacavin/wiresharebaryo-android/raw/main/assets/BARYO-VPN-poster.png" alt="BARYO VPN promotional preview" width="760">
  </a>
</p>

> **BARYO gives you a clear, reliable way to decide what travels through your VPN — from every app to one carefully selected group.**

---

## Start here

<table>
<tr>
<td width="33%" align="center">
<h3>1 · Download</h3>
Use the official APK button above or the release page.
</td>
<td width="33%" align="center">
<h3>2 · Install</h3>
Android 7.0+ is supported. Allow the normal Android install prompt.
</td>
<td width="33%" align="center">
<h3>3 · Connect</h3>
Import your profile, choose a routing mode and start the tunnel.
</td>
</tr>
</table>

> **Do not open the Code menu to download the app.** Use **Download APK** or the direct file link above.

## At a glance

| | Details |
|---|---|
| **Tunnel** | AmneziaWG userspace tunnel |
| **Package** | `com.wireshare.baryo` |
| **Version** | `1.6.30` · Build `39` |
| **Minimum Android** | Android 7.0 / API 24 |
| **Architectures** | ARM 32-bit, ARM 64-bit, x86, x86_64 |
| **Distribution** | Compiled APK only · no source code |

## Features

<table>
<tr>
<td width="50%" valign="top">

### Per-App control

- **All Apps** — route every installed app through the VPN.
- **Only Selected** — create a strict allowlist.
- **Exclude Selected** — route everything except bypassed apps.
- **Global policy** — keep one routing policy across every profile.
- Fast **Browsers / User / System** filters.
- Bulk select and clear actions with immediate tunnel re-application.

</td>
<td width="50%" valign="top">

### Security controls

- **Full Tunnel** with IPv4 and IPv6 default routes.
- **DNS anti-leak** with profile DNS and safe fallback handling.
- **Kill Switch** through Android Always-on VPN and lockdown.
- **App Bypass** for apps that must stay outside the tunnel.
- Defensive handling for incomplete or conflicting routes.

</td>
</tr>
</table>

## Choose the right routing mode

| Mode | Best for | Result |
|---|---|---|
| **All Apps** | Normal web browsing and full-device protection | Every app uses the VPN tunnel |
| **Only Selected** | A strict app allowlist | Only selected apps use the tunnel |
| **Exclude Selected** | A few apps must bypass the VPN | Everything else uses the tunnel |

> If websites do not open, check that the browser is not trapped in **Only Selected**. For ordinary browsing, start with **All Apps**.

## Security

### Recommended protection profile

1. Enable **Full Tunnel**.
2. Keep **DNS anti-leak** enabled.
3. Use **All Apps** for normal web browsing.
4. In Android settings, enable **Always-on VPN** and **Block connections without VPN** when you need fail-closed protection.
5. Import only profiles from sources you trust.

### Security and installation confidence

- Download only from this repository or the official GitHub release.
- Confirm the package name is `com.wireshare.baryo`.
- Verify the SHA-256 checksum before installing.
- The Android VPN permission dialog is expected because BARYO creates a local VPN tunnel.
- Avoid modified APKs from unknown websites, shortened links or unofficial channels.
- Never publish private keys, server credentials or complete VPN configurations.

## Privacy and data collection

**BARYO does not require an account and does not intentionally collect or send personal usage data to the developer.**

The current APK contains no advertising SDK, analytics SDK, crash-reporting service or tracking platform. Profiles, Per-App choices and tunnel settings are kept locally on your device. No browsing history, DNS history, app-usage report, private key or profile file is intentionally uploaded to a developer server.

> **VPN privacy note:** Your traffic still reaches the VPN server configured in your own profile. That server, its hosting provider and your network provider may have their own logging policies. Use a trusted server and keep private keys confidential.

This statement describes the current published APK. Review release notes and verify the checksum before installing future updates.

## Installation

### Android

1. Click **Download APK** at the top of this page.
2. Install the APK on an Android 7.0+ device.
3. If Android asks, allow installation from your browser or file manager.
4. Import your WireGuard or AmneziaWG profile.
5. Open **Settings → Per-App**, choose a routing mode and connect.

### ADB

```bash
adb install -r WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
```

## Verify the APK

```text
File:     WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
Version:  1.6.30
Build:    39
Package:  com.wireshare.baryo
SHA-256:  125989e7cb9c01624ec3bab5af9f294d71a21eff2cd343a99ec67387668861a4
```

<details>
<summary><b>Checksum commands</b></summary>

**Linux and macOS**

```bash
sha256sum WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
```

**Windows PowerShell**

```powershell
Get-FileHash .\WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk -Algorithm SHA256
```

</details>

## Compatibility

| Platform | Status |
|---|---|
| Android 7.0 Nougat / API 24 | Supported |
| Android 8.0 and newer | Recommended |
| ARM 32-bit / ARM 64-bit | Included |
| x86 / x86_64 | Included |

## Troubleshooting

| Symptom | First check |
|---|---|
| Websites do not open | Switch to **All Apps** or include the browser in **Only Selected**. |
| Only a few apps connect | Check whether the mode is set to **Only Selected**. |
| DNS appears outside the tunnel | Enable **DNS anti-leak** and verify profile DNS. |
| Traffic stops after disconnect | Review Android Always-on VPN and lockdown settings. |
| One profile behaves differently | Confirm the global Per-App policy is enabled. |

## Help shape the next release

<div align="center">

### Found a bug? Have an idea? Tell BARYO.

[![Report a Bug](https://img.shields.io/badge/REPORT%20A%20BUG-E53935?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Anooshacavin/wiresharebaryo-android/issues/new)
[![Request a Feature](https://img.shields.io/badge/REQUEST%20A%20FEATURE-1976D2?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Anooshacavin/wiresharebaryo-android/issues/new)

</div>

> **Your feedback directly improves BARYO.** Tell me what happened and I will investigate it. If you want a new capability, describe the use case and I will consider adding it to a future release.

When reporting a bug, include your Android version, device model, app version, build number, Per-App mode, reproduction steps and expected result. **Never post private keys or server credentials in a public issue.**

## Distribution

This public repository distributes the **compiled APK only**. Android source code, Gradle files, private keys, signing material and build internals are intentionally excluded.

[![Download the official APK](https://img.shields.io/badge/GET%20THE%20OFFICIAL%20APK-16A34A?style=for-the-badge&logo=android&logoColor=white)](https://github.com/Anooshacavin/wiresharebaryo-android/raw/main/download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk)

---

<div align="center">

**WIRE SHARE BARYO** · v1.6.30 · Build 39  
Designed and maintained by **Baryo**.

</div>
