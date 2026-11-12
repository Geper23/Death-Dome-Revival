# Compatibility & test checklist

**Reference environment:** Xiaomi Redmi (`tanzanite`), Android 15, DEATH DOME 2.1.2 / Revival V12.

These results were reported from real playtesting of the already-installed V12 build.

| Test | V12 result |
| --- | --- |
| App launch | ✅ Pass |
| Main menu navigation | ✅ Pass |
| First battle | ✅ Pass |
| Obsolete update check no longer blocks launch | ✅ Pass |
| Follow-up battles | ⏳ Not tested |
| Equipment, inventory, upgrades, shop | ⏳ Not tested |
| Saving after app restart | ⏳ Not tested |
| Clean XAPK install from phone | ⏳ Not tested |
| App update without save loss | ⏳ Not tested |
| Different Android devices | ⏳ Not tested |

## Suggested test sequence

1. Launch the game and confirm that startup completes.
2. Navigate the main menu and enter a combat encounter.
3. Complete several fights, unlock equipment, and verify upgrades and progression.
4. Exit the game completely, reopen it, and check saved progress.
5. Test installation on a separate phone or emulator without removing a known-good installation.
6. Check behavior after an in-place update only when the signing certificate is known to match.

## Report format

- **Device model / codename:**
- **Android version:**
- **Revival version:**
- **Installation:** clean / update; XAPK installer name if applicable
- **What happened:**
- **What should have happened:**
- **Steps to reproduce:**
- **Crash log:** sanitized relevant section if available

Avoid pasting raw logs containing identifiers, account data or unrelated private information.

## Status policy

- **Confirmed:** tested on a stated device/version.
- **Experimental:** working in limited conditions but not generally verified.
- **Untested:** no successful end-to-end evidence yet.

A successful test on one device should not be described as universal compatibility.
