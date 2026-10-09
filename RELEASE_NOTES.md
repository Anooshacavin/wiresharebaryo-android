# WIRE SHARE BARYO v1.6.41 — Build 50

## MTU AUTO stability rewrite

This release replaces the previous MTU AUTO runtime path with a stable, non-destructive calibration flow.

### Fixed at the root

- Removed the dashboard polling path that rebuilt the MTU AUTO screen and caused jumping/pulsing UI.
- Removed automatic reconnects caused only by idle traffic.
- A connected but idle tunnel remains connected; no traffic is not treated as an MTU failure.
- A candidate is confirmed only after real received traffic.
- Candidate advancement happens only after an actual tunnel start failure.
- The screen updates its state, current value, next value and progress bar in place.

### Manual MTU coordination

- Manual MTU is authoritative whenever MTU AUTO is disabled.
- Wi-Fi compatibility no longer silently overrides the manual value with 1280.
- Manual MTU and AUTO learning remain isolated per profile and network.

### UI states

`OFF · MANUAL` · `READY` · `TESTING` · `WAITING` · `LEARNED` · `LIMIT REACHED`

### Verification

- Package: `com.wireshare.baryo`
- Version: `1.6.41`
- Build: `50`
- Unit tests: 20 passed, 0 failed
- APK signature: verified with APK Signature Scheme v2
- SHA-256: `c95250f18886b2403f46ea0cb12e142a1f5aaa46d83cae3cd3b236ef10c4bce1`

## Download

[Download the official APK from this release](https://github.com/Anooshacavin/wiresharebaryo-android/releases/tag/v1.6.41)

```bash
adb install -r WIRESHAREBARYO-1.6.41-build50.apk
```

## Distribution

This public repository distributes the compiled APK and release documentation only. Android source code and private signing material are intentionally excluded.
