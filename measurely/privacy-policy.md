# Privacy Policy — Measurely: Sound, Level, Lux

Effective date: 19 October 2026 · Package `com.techdev.measurely` · Contact: tecdroiddeveloper@gmail.com

**In short:** Measurely measures sound, angle, light, motion and air pressure on your phone, and keeps what you record
there. There is no account and no server of ours. Microphone sound is analysed in memory to compute the level and
spectrum and is never recorded, saved or uploaded; camera frames are only shown on screen. The app does not use your
location. To fix crashes and understand how the app is used in general, it uses Google Firebase Crashlytics (crash
reports) and Firebase Analytics (basic app events such as app opens and screens viewed, with device identifiers
including the advertising ID). This version shows no ads and sells nothing. We never sell data.

## 1. What the app processes, and where
All processing happens on your device. What the app stores is kept only in its private storage (a local database and
settings), which other apps cannot read.

| Information | Why | Where it stays |
|---|---|---|
| Microphone sound (only after you allow the microphone) | To compute the sound level and the spectrum while a sound tool is open | Processed in memory and discarded within a fraction of a second. **Never recorded, saved or sent** |
| Camera preview (only if you turn on the inclinometer's camera sight and allow the camera) | To show what you aim at | Shown on screen only. **Never captured, saved or sent** |
| Sensor readings: accelerometer, gyroscope, magnetic field, light, air pressure, and humidity or temperature where your phone has those sensors | Live tools, sensor check | Processed on your phone |
| Recorded sessions: the numbers you choose to record (for example "52 dB at 21:40"), events above your threshold, and the title, place and notes you type | History, charts, noise reports | On your phone until you delete them or uninstall |
| Calibration values (sound offset, ruler scale, level offsets, lux factor, altimeter reference) | Correct readings on your phone | On your phone |
| The position you choose for true north and sun times: a city from a list built into the app, or coordinates you type | Magnetic declination and sun/moon calculations | On your phone (the app has no location permission) |
| Settings: theme, units, language, favourites | To remember your choices | On your phone |
| Crash reports and basic app events (Firebase, release builds only) | Fix crashes, understand general usage | Sent to Google Firebase (see 4) |

Measurely does not read your location, contacts, files, photos, messages, accounts or the list of your apps.

## 2. Permissions
- **Microphone** (`RECORD_AUDIO`) — for the sound meter, spectrum and noise recordings. Asked the first time you open a
  sound tool, with an explanation. The sound is analysed in memory only; no audio is ever stored or sent. You can
  refuse or turn it off in Android settings; the other tools keep working.
- **Camera** (`CAMERA`) — only for the inclinometer's optional camera sight. Asked only when you turn the sight on.
  Frames are shown on screen and never saved. You can refuse; the plain sight keeps working.
- Normal permissions granted at install without a prompt: internet and network state (Firebase and Google Play),
  vibration (haptic feedback), and advertising ID (Firebase Analytics). Libraries in the app may add related normal
  permissions (for example Android's ad-services permissions from the Google Mobile Ads SDK, or background-work
  permissions used by Android's WorkManager for widgets); they are not used to collect anything beyond what this
  policy describes.
- Measurely has **no location permission**, no notifications in this version, and no access to your storage: exports
  use Android's file picker.

## 3. Exports, backups and feedback
When you export a session (CSV, JSON or a PDF noise report), the file is created on your phone and saved only where
you choose with Android's file picker, or sent with the app you pick in the share sheet. A noise report contains the
readings, the place and notes you typed, your phone model, Android version and the calibration used; it goes only where
you send it. Android may include the app's settings and history in your own Google account backup if you turned device
backup on; that is handled by Android and Google, not by us. When you use "Contact us", your e-mail app opens with the
app version, Android version and phone model added so we can help; you decide whether to send it.

## 4. Third-party services
The app includes Google components that follow Google's privacy policy (https://policies.google.com/privacy):

- **Firebase Crashlytics** (release builds) — crash and error reports: stack traces, device model, Android version,
  app version, free memory and disk at the time, and a Crashlytics installation ID. https://firebase.google.com/support/privacy
- **Firebase Analytics** (release builds) — automatically collected events (first open, sessions, screens viewed)
  with an app instance ID and the advertising ID. Your readings, recordings, notes and audio are not sent.
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
Measurely is not directed at children under 13, and we do not knowingly collect personal information from them.

## 7. Keeping and deleting data
Your recordings and calibrations stay on your phone until you delete them. You can delete sessions in the app
(History, or Settings › Delete all sessions), or remove everything by uninstalling the app or via Android Settings ›
Apps › Measurely › Storage › Clear storage. Files you exported are not touched; delete them where you saved them.
Firebase keeps crash reports for about 90 days and analytics data according to its retention settings. To ask for
deletion of crash or analytics data, write to tecdroiddeveloper@gmail.com with the app instance ID shown in the app's
About screen. Deletion page: https://adhavpavan.github.io/app-privacy-policy/measurely/delete-data/

## 8. Security
App data is kept in Android's private app storage. Connections to Google services are encrypted (HTTPS). No audio,
camera image, reading or recording is sent anywhere by the app.

## 9. Changes
We may update this policy when the app changes, for example if a later version adds background noise logging with a
notification. The current version, with its effective date, is always in the app (menu › Privacy policy) and at
https://adhavpavan.github.io/app-privacy-policy/measurely/.

## 10. Contact
Questions or requests about privacy: tecdroiddeveloper@gmail.com
