# نصب WIRE SHARE BARYO

## دانلود رسمی

### [دانلود مستقیم APK نسخه 1.6.41 — Build 50](https://github.com/Anooshacavin/wiresharebaryo-android/raw/main/download/WIRESHAREBARYO-1.6.41-build50.apk)

- **Version:** 1.6.41
- **Build:** 50
- **Package:** `com.wireshare.baryo`
- **Minimum Android:** 7.0 / API 24
- **Architectures:** ARM, ARM64, x86, x86_64
- **Distribution:** Official APK only; source code is not published in this repository

## What changed

- MTU AUTO was rewritten to remove screen jumping and dashboard-driven rebuilds.
- Idle traffic never causes an automatic disconnect/reconnect.
- Candidate MTU values advance only after a real tunnel start failure.
- Received traffic verifies a candidate and updates the UI in place.
- Manual MTU is the authoritative value when MTU AUTO is disabled.
- Settings remain grouped into Connection, Network, DNS, Per-App, MTU AUTO, Backup, About and Diagnostics.

## نصب

1. APK را از لینک رسمی بالا دانلود کنید.
2. فایل را باز کنید و اجازه نصب از این منبع را در صورت درخواست Android فعال کنید.
3. برنامه را نصب و اجرا کنید.
4. پروفایل WireGuard یا AmneziaWG را وارد کنید.
5. برای استفاده از calibration، از Settings → MTU AUTO آن را به‌صورت دستی فعال کنید.

## نصب با ADB

```bash
adb install -r WIRESHAREBARYO-1.6.41-build50.apk
```

## بررسی SHA-256

```text
c95250f18886b2403f46ea0cb12e142a1f5aaa46d83cae3cd3b236ef10c4bce1
```

این repository فقط APK رسمی و مستندات انتشار را ارائه می‌کند؛ سورس، فایل‌های Gradle، کلیدهای خصوصی و build internals منتشر نشده‌اند.
