# NNOK TV Release

This repository hosts public update manifests and GitHub Release assets for NNOK TV.

## Update Manifests

- `apk/mobile.json`
- `apk/leanback.json`

The app reads the manifest for its current mode, compares `code` with the installed `versionCode`, and downloads the matching ABI APK from the release asset URLs.

## Release Asset Names

- `NNOK-mobile-arm64_v8a.apk`
- `NNOK-mobile-armeabi_v7a.apk`
- `NNOK-leanback-arm64_v8a.apk`
- `NNOK-leanback-armeabi_v7a.apk`

## Proxy Prefix Order

The app tries the original GitHub Release asset URL first, then proxy-prefixed URLs in manifest order:

1. `https://gh-proxy.com/`
2. `https://wget.la/`
3. `https://ghfast.top/`
