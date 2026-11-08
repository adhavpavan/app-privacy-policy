# Privacy Policy — Voice Recorder

Effective date: 1 November 2026 · Package `com.techdev.voicerecorder` · Contact: tecdroiddeveloper@gmail.com

**In short:** Voice Recorder makes, stores and edits recordings on your phone. There is no account and no server of ours. Audio, recording names and notes are never uploaded. The microphone is used only after you tap Record, and a notification stays visible for as long as it records. The app uses the internet only for anonymous crash reports, basic usage statistics and Google Play. Those reports never include your audio. We never sell data.

## 1. What the app processes, and where
All processing happens on your device. Library details are kept in the app's private storage, which other apps cannot read. The audio files themselves are saved in a folder on your phone.

| Information | Why | Where it stays |
|---|---|---|
| Microphone audio (only after you tap Record) | To make the recording you started | Saved as a file you own, in Recordings/Voice Recorder or a folder you choose. Never listened to by us and never uploaded |
| Recording names, folders, tags, markers and notes | Your library | On your phone, in the app's private database. Never uploaded |
| Settings | To remember your choices | On your phone |
| Crash reports and basic app events (Firebase, release builds) | Fix crashes, understand general usage | Sent to Google Firebase (see 4). Never includes audio, recording names or notes |

The app does not read your contacts, call log, location, messages, accounts or media library.

## 2. Permissions
- **Microphone** (`RECORD_AUDIO`) — only after you tap Record. A notification stays visible, with the recording indicator, for as long as the microphone is in use. You can refuse the permission; the library, player and editor still open.
- **Recording in the background** (`FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_MICROPHONE`) — so a recording you started keeps going with the screen off. It starts only from your tap, never from boot. The ongoing notification is how you see and stop it.
- **Playback in the background** (`FOREGROUND_SERVICE_MEDIA_PLAYBACK`) — so playback can continue with the screen off, with the usual media controls.
- **Notifications** (`POST_NOTIFICATIONS`, Android 13 and later) — asked when you first record, so that recording notification can be shown.
- **Bluetooth** (`BLUETOOTH_CONNECT`, Android 12 and later) — only if you pick a Bluetooth microphone or headset. Not used otherwise.
- **Storage** (`WRITE_EXTERNAL_STORAGE`) — Android 8 and 9 only, the first time a recording is saved into the shared Recordings folder. Android 10 and later do not use this permission.
- **Internet and network state** — Firebase Crashlytics, Firebase Analytics and Google Play only. Recording, playback and editing work fully offline.
- **Advertising ID** — used by Firebase Analytics in release builds. You can turn analytics off in Settings.
- The app asks for no contacts, call log, location or media-library permission.

## 3. Exports, backups and sharing
Recordings are saved to Recordings/Voice Recorder, or to a folder you choose. When you share a recording, Android's share sheet sends it only to the app you pick, under that app's own policy. Android's own backup may copy library details (names, folders, tags, markers, notes) and settings to your Google account if you turned backup on. Audio is never included in that backup. When you use Contact us, your e-mail app opens with the app version, Android version and phone model added so we can help; you decide whether to send it.

## 4. Third-party services
Release builds use Google services that follow Google's privacy policy (https://policies.google.com/privacy):

- **Firebase Crashlytics** — crash reports with device model, Android version, app version and app state, and a Crashlytics installation ID. https://firebase.google.com/support/privacy
- **Firebase Analytics** — basic, anonymous usage statistics such as app opens and which screens are used, with an app instance ID and the advertising ID. You can turn this off in Settings. Audio, recording names and notes are not sent.
- **Google Play in-app updates and in-app review** — to offer updates and, occasionally, a review prompt.
- **Google Play Billing** — for a Pro purchase. Google handles the payment; the app only learns whether Pro is owned by your Google account.
- **Google AdMob** — included for possible future ads, but turned off: no ads are shown and AdMob is never started. If ads are ever turned on, this policy will be updated first and the app will ask for consent where the law requires it.

## 5. Purchases
Pro is bought through Google Play Billing. Google handles the payment. The app only learns whether Pro is owned by your Google account.

## 6. Sharing and selling
We do not sell, rent or share personal data. Google processes the Firebase and Play data above as our service provider.

## 7. Children
The app is not directed at children under 13, and we do not knowingly collect personal information from them.

## 8. Keeping and deleting data
Recordings stay until you delete them. Deleted recordings wait in Trash for 30 days by default (7, 30 or 90 days in Settings), then they are removed. Uninstalling the app removes the library database and settings, but it keeps the audio files in Recordings/Voice Recorder; delete that folder yourself if you want the audio gone. Firebase keeps crash reports for about 90 days and analytics data according to its retention settings. To ask for deletion of crash or analytics data, write to tecdroiddeveloper@gmail.com with the app instance ID shown in the app's About screen. Deletion page: https://adhavpavan.github.io/app-privacy-policy/voice-recorder/delete-data/

## 9. Security
App data is kept in Android's private app storage, which other apps cannot read. Audio files you save sit in the folder you chose. Connections to Google services use encryption (HTTPS). No audio, recording name or note is sent over the internet by the app.

## 10. Changes
We may update this policy when the app changes. The current version, with its effective date, is always in the app (menu › Privacy policy) and at https://adhavpavan.github.io/app-privacy-policy/voice-recorder/.

## 11. Contact
Questions or requests about privacy: tecdroiddeveloper@gmail.com. When you use Contact us, your e-mail app adds the app version, Android version and phone model so we can help.
