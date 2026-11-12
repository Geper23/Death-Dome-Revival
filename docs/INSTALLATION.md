# Installation guide (planned XAPK distribution)

[Back to README](../README.md) · [Česká dokumentace](../README_CS.md)

> **The assembled Revival XAPK has not yet been verified with a clean installation.** The following describes the intended distribution workflow, rather than a completed compatibility test.

## What is an XAPK?

An XAPK is a single downloadable archive that usually bundles an Android APK and extra game files such as OBB. This is **not** a standalone APK: Android does not install an XAPK by tapping it with its standard APK package installer.

The Revival package is intended to contain:

```text
DEATH_DOME_REVIVAL_V12_ANDROID15.xapk
├── com.glu.ddome.apk
├── Android/obb/com.glu.ddome/
│   └── main.212.com.glu.ddome.obb
├── icon.png
└── manifest.json
```

The exact XAPK name can change. The APK and patched OBB must match.

## Android installation (no USB or PC required)

1. Download the authorized, tested release XAPK when it becomes available.
2. Install or open an XAPK-compatible installer capable of placing OBB content correctly on your Android version.
3. Open the downloaded XAPK with that installer.
4. Confirm the Android installation prompts.
5. Launch DEATH DOME and test startup, menu, combat and game progress.

Because Android storage rules and installer capabilities vary, installation can behave differently across devices. **Do not assume all XAPK installers can place OBB data on Android 15.**

## Protect your saved game

- Do not uninstall a working build just to test a new installer.
- Updating an APK requires the same signing certificate as the already installed package; otherwise the update can fail.
- Copying APK and OBB is **not** the same as backing up the game's private saved data.
- Do not clear app data unless you accept the risk of losing progress.

## Troubleshooting

**Game opens but gets stuck on startup:** verify the correct *patched* OBB was installed, and report the Android version and exact symptoms.

**Installation fails because of signature mismatch:** an existing installation may use a different signing certificate. Do **not** uninstall it before saving your progress.

**XAPK installer does not place OBB:** try a compatible installer that explicitly supports OBB on your Android version; report the installer version and Android version.

**Crash:** provide the device model, Android version, whether it was a clean install, exact reproduction steps, and sanitized `logcat` output.

## Distribution rights

Only share game APK/OBB files where you hold the necessary distribution rights or permission. This repository contains documentation, not a license to original game assets.
