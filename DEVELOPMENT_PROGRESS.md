# KARTLY (Smart Grocery & Pantry Management) - Android - Development Progress

Current package: Version 3.1 (versionName 3.1.0, versionCode 31). Designed by CB.

## Milestones
| # | Milestone | Status |
|---|---|---|
| M1 | v2.4 base: signing key, compact layouts, partial-purchase aids | DONE |
| M2 | v3.0: KARTLY branding, cart logo, animated splash, partial-purchase fix in Available Items | DONE |
| M3 | v3.1: complete UI redesign (navy / emerald / amber palette, bottom navigation with a More sheet, page headers, item cards, search row with collapsible Filters), pencil background art removed, Designed by CB + version top-left, simplified splash (logo, KARTLY, Kannada line), delete for available items (single and bulk, with confirmation), Save buttons on Available Items and Shopping List, backup reminder and last-backup tracking, add forms moved to the bottom (collapsible), tab order Add Items, Shopping List, Available Items, Medicines, Stationery, Expire items, KPI, Data | DONE (tested in headless Chromium at phone size; APK build not run here) |
| M4 | Device test of the built APK, fixes | PENDING (needs user feedback) |
| M5 | Bill photo reading and Kannada translation for names outside the catalog (needs decision: own API key vs offline) | PENDING |
| M6 | Signed release APK instructions | PENDING |

## How data is protected
- All lists are saved on the phone automatically (browser storage inside the app) after every change.
- Save button (Available Items, Shopping List) and Back up now (Add Items banner, Data & Templates) create a JSON backup and open the Android share sheet so a copy can go to Drive, Files or WhatsApp. The date of the last backup is recorded and shown; a reminder appears on Add Items after 7 days without a backup.
- Restore from backup (Data & Templates) reads the JSON file back.

## Known issues and notes
- Installing over 2.3.1 is not possible (different signing key). From 3.0 on, builds use signing/grocery-debug.keystore and update in place. Keep that file in the repository.
- Bill photo reading is not available in the Android build yet.
- APK build and phone testing for 3.1 not yet done.

## Resume rule
New session: read this file and continue from the first milestone not marked DONE.
