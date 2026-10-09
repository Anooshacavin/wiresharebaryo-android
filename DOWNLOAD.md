# نصب WIRE SHARE BARYO

## دانلود رسمی

### [دانلود مستقیم APK نسخه 1.6.42 — Build 51](https://github.com/Anooshacavin/wiresharebaryo-android/raw/main/download/WIRESHAREBARYO-1.6.42-build51.apk)

- **Version:** 1.6.42
- **Build:** 51
- **Package:** `com.wireshare.baryo`
- **Minimum Android:** 7.0 / API 24
- **Distribution:** Official APK only; source code is not published in this repository

## قابلیت جدید: wireguard://

در بخش **Profiles → Create profile** می‌توانید یک WireGuard share URI را وارد کنید. BARYO آن را به‌صورت محلی به کانفیگ معتبر تبدیل و قبل از ذخیره validate می‌کند.

پشتیبانی شامل private key، server host/port، address، public key، MTU، DNS، AllowedIPs، pre-shared key، persistent keepalive و نام پروفایل از fragment است.

پارامترهای reserved شناسایی و به‌عنوان metadata حفظ می‌شوند؛ اعمال reserved bytes سفارشی به پشتیبانی native/backend وابسته است.

## تغییرات نسخه 1.6.42

- پشتیبانی از واردکردن wireguard:// در فرم دستی
- تبدیل URI فقط روی دستگاه و بدون ارسال به سرویس خارجی
- اعتبارسنجی URI قبل از ذخیره
- حفظ پشتیبانی کامل از فایل‌های .conf
- MTU AUTO پایدار، بدون پرش صفحه و reconnect ناشی از idle traffic
- Manual MTU هنگام خاموش‌بودن AUTO مرجع قطعی باقی می‌ماند

## نصب

1. APK رسمی بالا را دانلود کنید.
2. در صورت درخواست Android، اجازه نصب از این منبع را فعال کنید.
3. برنامه را نصب و اجرا کنید.
4. از Profiles یک فایل .conf یا یک wireguard:// URI وارد کنید.

## نصب با ADB

```bash
adb install -r WIRESHAREBARYO-1.6.42-build51.apk
```

## SHA-256

```text
f5f9918382dc7d72c38c8002c1afca45bc90264bcb7a429fafc6394d7ebce3b6
```

این repository فقط APK رسمی و مستندات انتشار را ارائه می‌کند؛ سورس، کلیدهای خصوصی و build internals منتشر نشده‌اند.
