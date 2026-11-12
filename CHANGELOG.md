# Development history — DEATH DOME REVIVAL

**Game baseline:** DEATH DOME 2.1.2 · **Current working patch:** V12  
**Scope:** Experimental Android 15 compatibility research; not all builds are public releases.

The version numbers below document the **repair process**, not twelve published stable releases. Findings are based on debugging and testing on a Xiaomi Redmi (`tanzanite`) running Android 15.

## V12 — first confirmed playable build ✅

- Removed a legacy `MobileAppTracker.getDeviceId(Context)` dependency on restricted telephony device identifiers.
- Tester confirmed the game launches, the main menu works, and the first battle completes.
- **Remaining:** longer gameplay, saves, and clean XAPK installation need confirmation.

## V11 — legacy preferences fix

- Updated a legacy PlayHaven preferences access mode to avoid `MODE_WORLD_WRITEABLE no longer supported`.
- Revealed a subsequent `MobileAppTracker` device-ID restriction at runtime.

## V10 — modified APK signing compatibility

- Addressed signature verification in the experimental, test-signed APK.
- The prior “Not a genuine copy” rejection no longer appeared in testing.
- This was **not yet playable**: an outdated PlayHaven API call still crashed.

## V9 — native device-ID compatibility

- Adjusted three outdated native device-ID access paths in `libgwallet.so`.
- Removed the previously observed native device-ID abort.
- A separate signature-check problem still prevented normal use.

## V8 — first native device-ID attempt

- Experimental patch for restricted device-ID behavior.
- Not sufficient to resolve the crash.
- A signing-key change required a clean install during this stage. Subsequent V8–V12 test builds used a consistent signature to support in-place updates.

## V7 — obsolete update service

- Modified legacy game configuration so unreachable update-server checks no longer blocked startup.
- Game proceeded further but hit native device-ID and copy-validation problems.

## V6 — Android bytecode verification

- Repaired a verifier failure introduced while addressing obsolete billing-service behavior.
- Game could load further but waited on unavailable legacy update endpoints.

## V5 — initial billing-service patch

- Attempted to handle outdated Google Play billing service use.
- Exposed a bytecode verifier issue; this build was not a usable release.

## V4 — legacy billing crash identified

- Game advanced past startup/cutscene; encountered `Service Intent must be explicit`.

## V1–V3 — initial compatibility research

- Investigated original APK/XAPK and native-library compatibility on Android 15.
- Early experiments addressed startup issues; these are not validated playable releases.

## Verification status

| Test | Status |
| --- | --- |
| Android 15 app launch | Confirmed in V12 |
| Main menu | Confirmed in V12 |
| First combat encounter | Confirmed in V12 |
| Full story / subsequent fights | Not verified |
| Saves after reinstall | Not verified |
| Clean XAPK setup | Not verified |
| Compatibility on other phones | Not verified |

**Note:** This document is a technical development summary, not a promise that every original online service, purchase or game feature works.
