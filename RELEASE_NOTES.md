# WIRE SHARE BARYO v1.6.42 — Build 51

## wireguard:// URI import

The manual Create/Edit Profile form now accepts common WireGuard share URIs and converts them locally into validated WireGuard/AmneziaWG configuration text.

### Supported URI data

- Interface private key from URI userinfo
- Server host and port
- Address
- Peer public key
- MTU
- DNS
- AllowedIPs
- PreSharedKey
- PersistentKeepalive
- Profile name from the URI fragment

The URI is never sent to a remote service. It is converted locally and only the resulting profile is stored in the app-private profile directory. The sample URI from the request is not included in the source, tests, APK documentation or GitHub repository.

### Reserved parameter

The parser recognizes reserved bytes and preserves them as metadata. The current backend does not apply custom reserved bytes at the native transport layer, so servers that require non-standard reserved bytes may need a future native/backend extension.

## MTU AUTO stability carried forward

- No dashboard-driven screen rebuilds during polling.
- Idle traffic never triggers disconnect/reconnect.
- Candidates advance only after actual tunnel start failure.
- Received traffic confirms a candidate.
- Manual MTU remains authoritative when AUTO is disabled.

## Verification

- Package: `com.wireshare.baryo`
- Version: `1.6.42`
- Build: `51`
- Unit tests: 23 passed, 0 failed
- APK signature: verified with APK Signature Scheme v2
- SHA-256: `f5f9918382dc7d72c38c8002c1afca45bc90264bcb7a429fafc6394d7ebce3b6`

## Download

[Download the official APK from this release](https://github.com/Anooshacavin/wiresharebaryo-android/releases/tag/v1.6.42)

```bash
adb install -r WIRESHAREBARYO-1.6.42-build51.apk
```

## Distribution

This public repository distributes the compiled APK and release documentation only. Android source code and private signing material are intentionally excluded.
