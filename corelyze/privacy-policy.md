# Privacy Policy — Corelyze: CPU & Device Info

Effective date: 17 October 2026 · Package `com.techdev.corelyze` · Contact: tecdroiddeveloper@gmail.com

**In short:** Corelyze reads your phone's hardware and software details on the phone itself and shows them to you.
There is no account and no server of ours, and your device information is never uploaded. To fix crashes and
understand how the app is used in general, the app uses Google Firebase Crashlytics (crash reports) and Firebase
Analytics (basic app events such as app opens and screens viewed, with device identifiers including the advertising
ID). Pro is bought through Google Play. We never sell data.

## 1. What the app processes, and where
All processing happens on your device. Anything the app stores is kept only in its private storage (local database
and settings), which other apps cannot read.

| Information | Why | Where it stays |
|---|---|---|
| Hardware and software details from Android and the phone: model, chip (SoC), CPU, GPU, memory, storage, battery, display, cameras (specifications only), sensors, network status, Android build, security patch, codecs, DRM, system features | To show them to you, explain them and build reports | On your phone |
| Live values: CPU clock speeds, battery current/voltage/temperature, thermal status, memory use, network speed | Live screens and widgets | In memory; on your phone |
| List of launchable apps and their package details (versions, target SDK, install source, requested permissions, components, signing-certificate fingerprint) | Apps screens and insights | On your phone |
| Hardware test results (pass/fail, plus measured facts such as GPS time-to-fix and satellite count — never your position), benchmark results | Reports and history | On your phone |
| Battery history: charging sessions and battery level, current, voltage, temperature and thermal status, sampled while the app is open and about every 15 minutes in the background. You can turn it off and clear it in the app | Battery health estimate, history charts, charge alarm, overheat alert | On your phone (kept 7 days, or until you clear it with Pro) |
| Optional Shizuku mode (only if you install the separate Shizuku app and allow Corelyze in it): CPU usage, names and CPU/memory use of running processes, hidden temperature sensors, battery service details | To show real CPU usage and values Android hides from apps. Corelyze only reads; you can revoke the access in Shizuku at any time | In memory, on screen only; never stored or sent |
| Storage speed test file (deleted right after the test) and charger test results with the charger names you type | Storage speed and charger comparison | On your phone |
| Notes you type into a buyer report | Printed in that PDF only | On your phone |
| Settings (theme, units, battery calibration) and whether Pro is unlocked | To remember your choices | On your phone |
| Crash reports and basic app events (Firebase, release builds only) | Fix crashes, understand general usage | Sent to Google Firebase (see 4) |

Unknown chips: when the built-in database doesn't know your chip, the crash-reporting service receives the chip's
model code, board name and CPU part ids (hardware identifiers only, no personal data) so a later update can add it.

## 2. Permissions
Corelyze needs no permission to show device information. These optional permissions are requested only when you
tap the feature that needs them; you can refuse or revoke them at any time.

- **Notifications** — only for the charge alarm and overheat alert you turn on.
- **Precise location** — Android requires it to show your Wi-Fi network name and for the GPS test. Used only while
  the screen is open, never in the background, never stored or sent.
- **Phone** — to show SIM details such as the data network type. The app never reads your phone number, IMEI or
  other identifiers.
- **Camera** — camera test preview, colour picker and magnifier: live preview only. Nothing is recorded or saved. (Camera specifications need no permission.)
- **Microphone** — microphone test (records 3 seconds, plays it back and deletes it) and sound meter (live level only, nothing recorded).
- Normal permissions declared without prompts: internet and network state (Firebase, Google Play), Wi-Fi state
  (Wi-Fi details), vibration and biometrics (hardware tests), run at startup (re-schedule widget refresh), advertising
  ID (Firebase Analytics).

## 3. Exports, sharing and feedback
When you copy, share or export information (text, PDF, JSON), the file is created on your phone and goes only where
you send it. Reports contain device details, not personal data, unless you add your own notes. When you use
"Contact us", your e-mail app opens with the app version, Android version and phone model added so we can help.

## 4. Third-party services
The app includes Google components that follow Google's privacy policy (https://policies.google.com/privacy):

- **Firebase Crashlytics** (release builds) — crash and error reports: stack traces, device model, Android version,
  app version, free memory/disk at the time, a Crashlytics installation ID.
  https://firebase.google.com/support/privacy
- **Firebase Analytics** (release builds) — automatically collected events (first open, sessions, screens viewed,
  in-app purchase events) with an app instance ID and the advertising ID. No device-info values are logged.
- **Google Play Billing** — the one-time Pro purchase. Google handles payment; the app only learns whether your Google
  account owns Pro.
- **Google Play in-app updates and in-app review** — to offer updates and, occasionally, a review prompt.
- **Google AdMob and User Messaging Platform** — included but **turned off**: no ads are shown and AdMob is never
  started. If ads are ever turned on, this policy and an in-app consent screen will say so first.

## 5. Sharing and selling
We do not sell, rent or share personal data. Google processes the Firebase and Play data above as our service
provider.

## 6. Children
Corelyze is not directed at children under 13, and we do not knowingly collect personal information from them.

## 7. Keeping and deleting data
Data stored by the app stays on your phone until you delete it; uninstalling the app or clearing its storage removes
all of it. Firebase keeps crash reports for about 90 days and analytics data according to its retention settings.
To ask for deletion of crash or analytics data, write to tecdroiddeveloper@gmail.com. Deletion page:
https://adhavpavan.github.io/app-privacy-policy/corelyze/delete-data/

## 8. Security
App data is kept in Android's private app storage. Connections to Google services are encrypted (HTTPS).

## 9. Changes
We may update this policy when the app changes. The current version, with its effective date, is always in the app
(menu → Privacy policy) and at https://adhavpavan.github.io/app-privacy-policy/corelyze/.

## 10. Contact
Questions or requests about privacy: tecdroiddeveloper@gmail.com
