# WIRE SHARE BARYO v1.6.30

## Per-App filter bugfix

- Fixed delayed filter switching in Settings → Per-App.
- Fixed empty BROWSERS results on Android 11+ package visibility rules.
- Added Android browser intent discovery for more reliable browser detection.
- Filter buttons update immediately without rebuilding the entire Settings page.
- Preserved ALL APPS, ONLY SELECTED, EXCLUDE SELECTED, global policy and profile policy behavior.

## Security capabilities already included

- Full Tunnel with IPv4/IPv6 default routes.
- App Bypass through EXCLUDE SELECTED.
- DNS anti-leak fallback.
- Kill Switch / Android Lockdown integration.

## Install

Download the APK from `releases/v1.6.30/` and install:

```bash
adb install -r WIRESHAREBARYO-1.6.30-build39-perapp-fix.apk
```

SHA-256:

```text
125989e7cb9c01624ec3bab5af9f294d71a21eff2cd343a99ec67387668861a4
```
