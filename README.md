<p align="center">
  <img src="assets/BARYO-VPN-poster.png" alt="BARYO VPN" width="680">
</p>

<h1 align="center">WIRE SHARE BARYO</h1>

<p align="center">
  <strong>Secure AmneziaWG VPN control for Android</strong><br>
  <sub>Private networking · Precise app routing · Complete control</sub>
</p>

<p align="center">
  <a href="https://github.com/Anooshacavin/wiresharebaryo-android/raw/refs/heads/main/download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk"><img src="https://img.shields.io/badge/⬇%20DOWNLOAD%20APK-2563EB?style=for-the-badge&logo=android&logoColor=white" alt="Download APK"></a>
  <a href="DOWNLOAD.md"><img src="https://img.shields.io/badge/INSTALL%20GUIDE-0EA5E9?style=for-the-badge&logo=readme&logoColor=white" alt="Installation guide"></a>
  <a href="RELEASE_NOTES.md"><img src="https://img.shields.io/badge/RELEASE%20NOTES-7C3AED?style=for-the-badge&logo=git&logoColor=white" alt="Release notes"></a>
</p>

---

## ⬇️ دانلود APK

### برای نصب برنامه، روی دکمه‌ی سبز زیر کلیک کنید

<p align="center">
  <a href="https://github.com/Anooshacavin/wiresharebaryo-android/raw/refs/heads/main/download/WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk"><img src="https://img.shields.io/badge/⬇%20DOWNLOAD%20APK%20-%20%D8%AF%D8%A7%D9%86%D9%84%D9%88%D8%AF%20%D9%85%D8%B3%D8%AA%D9%82%DB%8C-16A34A?style=for-the-badge&logo=android&logoColor=white" alt="Download APK"></a>
</p>

**English:** Click the green **DOWNLOAD APK** button above. You do not need to open the `Code` menu or download the repository files.

<p align="center">
  <img src="https://img.shields.io/badge/Android-7.0%2B-22C55E?style=flat-square&logo=android&logoColor=white" alt="Android 7.0+">
  <img src="https://img.shields.io/badge/Release-v1.6.30-F97316?style=flat-square" alt="Release v1.6.30">
  <img src="https://img.shields.io/badge/Build-39-EC4899?style=flat-square" alt="Build 39">
  <img src="https://img.shields.io/badge/Distribution-APK%20Only-8B5CF6?style=flat-square" alt="APK only">
</p>

> **WIRE SHARE BARYO** is authored and maintained by **Baryo** — focused on dependable Android VPN control, advanced Per-App routing and privacy-first networking.

## Why BARYO?

| | Capability | What it gives you |
|---|---|---|
| 🔵 | **Full Tunnel** | Route IPv4 and IPv6 traffic through the VPN. |
| 🟣 | **Per-App Control** | Choose All Apps, Only Selected or Exclude Selected. |
| 🟢 | **DNS Anti-Leak** | Keep DNS traffic aligned with the active tunnel. |
| 🟠 | **Kill Switch** | Support fail-closed Android VPN behavior. |
| 🔷 | **Global Policy** | Keep one Per-App policy across every profile. |

## Feature dashboard

### 🛡️ Secure tunnel controls

- **AmneziaWG userspace tunnel** for modern WireGuard-compatible profiles.
- **Full Tunnel** with IPv4 and IPv6 default routes.
- **DNS anti-leak** using profile DNS with a safe fallback.
- **Kill Switch** support through Android Always-on VPN and lockdown settings.
- **App Bypass** for applications that must stay outside the tunnel.

### 🎛️ Advanced Per-App routing

- **All Apps** — route every installed application through the VPN.
- **Only Selected** — route only the applications you choose.
- **Exclude Selected** — protect everything except bypassed applications.
- **Global policy** — keep the same policy synchronized across all profiles.
- **Fast filters** — All, Browsers, User Apps and System Apps.
- **Browser presets** — quickly protect or bypass detected browsers.
- **Bulk selection** — select or clear visible apps in one tap.

## Quick start

1. Download the APK from the blue button above.
2. Install it on an Android 7.0+ device.
3. Import your WireGuard/AmneziaWG profile.
4. Open **Settings → Per-App**.
5. Choose **All Apps**, **Only Selected** or **Exclude Selected**.
6. For stronger protection, enable **Always-on VPN** and **Block connections without VPN** in Android settings.

> **Recommended setup:** Enable **Full Tunnel** and **DNS anti-leak**. For normal web browsing, use **All Apps** or **Protect browsers**.

## Compatibility

| Requirement | Supported |
|---|---|
| Minimum Android | **7.0 Nougat / API 24** |
| Recommended Android | **8.0 or newer** |
| ARM 32-bit | ✅ Included |
| ARM 64-bit | ✅ Included |
| x86 / x86_64 | ✅ Included |
| Package name | `com.wireshare.baryo` |

## Installation

### Direct installation

1. Open [DOWNLOAD.md](DOWNLOAD.md).
2. Download the latest APK.
3. If Android asks, allow installation from your browser or file manager.
4. Install the APK and import your profile.

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

**Linux / macOS**

```bash
sha256sum WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
```

**Windows PowerShell**

```powershell
Get-FileHash .\WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk -Algorithm SHA256
```

## Troubleshooting

| Problem | Fix |
|---|---|
| Websites do not open | Set Per-App to **All Apps** or enable **Protect browsers**. |
| Only selected apps connect | Check that the mode is not set to **Only Selected** unintentionally. |
| DNS appears outside the tunnel | Enable **DNS anti-leak** and verify profile DNS. |
| Traffic stops after disconnect | Review Android Always-on VPN and lockdown settings. |
| One profile behaves differently | Confirm that the global Per-App policy is enabled. |

When reporting a problem, include your Android version, device model, app build, affected profile count and Per-App mode. Never upload private keys, server credentials or unsanitized VPN configurations.

## Distribution

This public repository distributes the **compiled APK only**. Android source code, Gradle files, private keys, signing material and build internals are intentionally excluded.

The APK is provided for personal testing and use. Do not upload private configuration files or credentials.

<p align="center">
  <br>
  <strong>Designed and maintained by Baryo</strong><br>
  <sub>WIRE SHARE BARYO · v1.6.30 · Build 39</sub>
</p>
