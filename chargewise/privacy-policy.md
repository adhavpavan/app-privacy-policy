# Privacy Policy — Chargewise: Battery Health

Effective date: 19 October 2026 · Package `com.techdev.chargewise` · Contact: tecdroiddeveloper@gmail.com

**In short:** Chargewise reads your phone's battery information on the phone itself and keeps your battery history
there. There is no account and no server of ours, and your battery data is never uploaded. To fix crashes and
understand how the app is used in general, the app uses Google Firebase Crashlytics (crash reports) and Firebase
Analytics (basic app events such as app opens and screens viewed, with device identifiers including the advertising
ID). This version shows no ads and sells nothing. We never sell data.

## 1. What the app processes, and where
All processing happens on your device. What the app stores is kept only in its private storage (a local database and
settings), which other apps cannot read.

| Information | Why | Where it stays |
|---|---|---|
| Battery readings from Android: level, charging status, plug type, current, voltage, temperature, charge counter, cycle count and battery facts where your phone reports them, thermal status, and whether the screen is on | Live screens, widgets, the Quick Settings tile, alarms and alerts | On your phone |
| Battery history: charge and discharge sessions built from those readings, sampled often while the app is open and from time to time in the background | Session history and curves, health estimate, wear meter, charging summaries | On your phone until you clear it in the app or uninstall |
| Health estimate, learned battery capacity, cycle estimate and current-calibration result | To show your battery's health and correct readings on your phone | On your phone |
| Your phone model, used to look up the battery's design capacity in a database built into the app; or the capacity you type | Health % | On your phone (the lookup happens inside the app; nothing is sent) |
| Alarm and alert settings, theme, units and language | To remember your choices | On your phone |
| Crash reports and basic app events (Firebase, release builds only) | Fix crashes, understand general usage | Sent to Google Firebase (see 4) |

Chargewise does not read your location, contacts, files, photos, messages, accounts or the list of your apps.

## 2. Permissions
Chargewise needs no permission to show battery information.

- **Notifications** (Android 13 and newer) — only to ring the charge alarms and show the alerts you turn on. Asked the
  first time you turn one on. You can refuse or turn it off in Android settings; the rest of the app keeps working.
- Normal permissions granted at install without a prompt: internet and network state (Firebase and Google Play),
  run at startup (to restart background battery checks after a reboot), vibration (alarm vibration), keep the
  processor awake briefly and background work (used by Android's WorkManager to run the background battery checks),
  and advertising ID (Firebase Analytics).

## 3. Exports, backups and feedback
When you export your history as a CSV file, the file is created on your phone and saved only where you choose with
Android's file picker; it goes only where you send it. Android may include the app's settings and history in your
own Google account backup if you turned device backup on; that is handled by Android and Google, not by us. When you use
"Contact us", your e-mail app opens with the app version, Android version and phone model added so we can help; you
decide whether to send it.

## 4. Third-party services
The app includes Google components that follow Google's privacy policy (https://policies.google.com/privacy):

- **Firebase Crashlytics** (release builds) — crash and error reports: stack traces, device model, Android version,
  app version, free memory and disk at the time, and a Crashlytics installation ID. https://firebase.google.com/support/privacy
- **Firebase Analytics** (release builds) — automatically collected events (first open, sessions, screens viewed)
  with an app instance ID and the advertising ID. Your battery readings and history are not sent.
- **Google Play in-app updates and in-app review** — to offer updates and, occasionally, a review prompt.
- **Google Play Billing** — included for a possible future one-time "Pro" purchase, but **not active in this version**:
  every feature is free and nothing can be bought.
- **Google AdMob and User Messaging Platform** — included for possible future ads, but **not active in this version**:
  no ads are shown and AdMob is never started. If ads or purchases are ever turned on, this policy will be updated
  first and the app will ask for consent where the law requires it.

## 5. Sharing and selling
We do not sell, rent or share personal data. Google processes the Firebase and Play data above as our service
provider.

## 6. Children
Chargewise is not directed at children under 13, and we do not knowingly collect personal information from them.

## 7. Keeping and deleting data
Your battery history stays on your phone until you delete it. You can clear it in the app (Settings), or remove
everything by uninstalling the app or via Android Settings › Apps › Chargewise › Storage › Clear storage. Firebase keeps
crash reports for about 90 days and analytics data according to its retention settings. To ask for deletion of crash
or analytics data, write to tecdroiddeveloper@gmail.com with the app instance ID shown in the app's About screen.
Deletion page: https://adhavpavan.github.io/app-privacy-policy/chargewise/delete-data/

## 8. Security
App data is kept in Android's private app storage. Connections to Google services are encrypted (HTTPS). No battery data
is sent anywhere.

## 9. Changes
We may update this policy when the app changes, for example when a new feature reads new data. The current version, with
its effective date, is always in the app (menu › Privacy policy) and at https://adhavpavan.github.io/app-privacy-policy/chargewise/.

## 10. Contact
Questions or requests about privacy: tecdroiddeveloper@gmail.com
