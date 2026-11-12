# DEATH DOME REVIVAL

**Bringing the original DEATH DOME (Android 2.1.2) back to modern Android devices.**

[Česky / Czech README](README_CS.md) · [Installation guide](docs/INSTALLATION.md) · [Compatibility & testing](docs/TESTING.md) · [Changelog](CHANGELOG.md)

> **Status: V12 — playable experimental build.** The main menu and first fight have been verified on one Android 15 phone. A clean XAPK installation and full game progression have **not** yet been verified.

## About the project

**DEATH DOME REVIVAL** is an independent, unofficial game-preservation and compatibility effort focused on running the original mobile game on newer Android versions. Our goal is to retain the original gameplay, combat and atmosphere—not to remake or replace the game.

This repository currently contains **documentation and testing information**. The owner will publish Releases separately when they are ready.

## Current compatibility

| Area | Result | Evidence |
| --- | --- | --- |
| Android 15 launch | ✅ Confirmed | Xiaomi Redmi, device codename `tanzanite` |
| Main menu | ✅ Confirmed | Navigation tested in-game |
| Combat | ✅ Confirmed | First battle completed |
| Offline startup | ✅ Confirmed | Legacy update check no longer blocks startup |
| Other battles / full campaign | 🧪 Untested | More playtesting required |
| Saves across reinstall | 🧪 Untested | Preserve your working installation |
| Clean XAPK installation | 🧪 Untested | Installer + OBB placement still need verification |
| Other phones / Android versions | 🧪 Untested | No general compatibility guarantee |

**Test baseline:** DEATH DOME 2.1.2 / Revival patch V12 on Android 15. V12 is the first confirmed playable build, **not** a production-stable release across devices.

## What has been addressed?

The experimental V1–V12 repair effort investigated and addressed startup blockers involving:

- Older native Android/Unity runtime behavior.
- Obsolete update-server requests that could prevent game startup.
- Android restrictions on reading device identifiers.
- Deprecated third-party SDK behavior (including legacy preferences access).
- Signature compatibility for the test-signed build.

See [CHANGELOG.md](CHANGELOG.md) for a careful version-by-version summary.

## Installation

The planned player-facing package is **XAPK**: one downloadable archive containing the APK and its required OBB data. **Players should not need USB or ADB**, but an Android installer supporting XAPK with OBB placement is required.

1. Download an authorized, tested Revival XAPK release when available.
2. Open it using a compatible XAPK installer on your phone.
3. Follow the Android installation prompts.
4. Launch the game and test the menu, combat and saving.

**Important:** XAPK is not the same as a standalone APK. We have **not yet confirmed a clean install** of the newly assembled Revival XAPK. Do not uninstall a working V12 installation without a full backup of your app data.

Read the [full installation guide](docs/INSTALLATION.md).

## Known limitations

- Original online services, purchases, analytics, cloud saves and similar features may be unavailable.
- Later levels, inventory, shop features and long-term saving still need testing.
- Some Android versions and third-party XAPK installers may behave differently.
- Backing up APK + OBB alone does **not** preserve internal game saves.

## Bugs and testing

Use [GitHub Issues](../../issues) to report reproducible problems. Include your Android version, phone model, Revival version, installation method, steps to reproduce and a relevant crash log if available. **Remove personal information from logs before posting.**

See [Testing & compatibility](docs/TESTING.md).

## Legal / trademarks

DEATH DOME, its original game files, art, code, and trademarks remain the property of their respective rights holders. This is a **non-official fan compatibility/preservation project**, not affiliated with, authorized by or endorsed by Glu Mobile or any successor rights holder.

**Do not redistribute original APK, OBB, game assets or other copyrighted materials without appropriate permission.** This repository does not grant a license to proprietary game content.

---

**Maintained by [Geper23](https://github.com/Geper23).** Our priority is honest, device-verified preservation of the original experience.
