# Privacy Policy — Decibly: Sound Meter & dB

Effective date: 25 October 2026 · Package `com.techdev.decibly` · Contact: tecdroiddeveloper@gmail.com

**In short:** Decibly measures sound levels on your phone and keeps what you record there. There is no account and no
server of ours. Microphone sound is turned into levels in memory and is never uploaded. The only audio the app can
save is an optional event clip (about 10 seconds around a loud event), which is off by default, stays in the app's
private storage on your phone, is never uploaded and is never in a backup. The app does not use your location. To fix
crashes and understand how the app is used in general, it uses Google Firebase Crashlytics (crash reports) and
Firebase Analytics (basic app events such as app opens and screens viewed, with device identifiers including the
advertising ID). This version shows no ads and sells nothing. We never sell data.

## 1. What the app processes, and where
All processing happens on your device. What the app stores is kept only in its private storage (a local database, the
settings and, if you turn them on, event clips), which other apps cannot read.

| Information | Why | Where it stays |
|---|---|---|
| Microphone sound (only after you allow the microphone) | To compute the sound level, spectrum and octave bands while the meter, analyzer, mic check or a logging session runs, including a session you chose to keep running with the screen off or a night watch you armed (both shown by an ongoing notification with a Stop button) | Processed in memory and discarded within a fraction of a second. Only the numbers are saved. **Never uploaded** |
| Event clips (only if you turn on Settings › Save event clips; off by default) | To let you replay what a loud event sounded like | About 10 seconds of audio per event (4 s before, 6 s after), a WAV file of about 1 MB, in the app's private storage on your phone. At most 40 per session, and none when less than 200 MB is free. **Never uploaded, never in a backup, never copied to a new phone** |
| Sessions: 1-second levels, events above your threshold, octave band levels, the name, place and notes you type, and spot measurements | Reports, charts, comparisons, exports | On your phone until you delete them or uninstall |
| Calibration profiles: offsets, mic check results, the date and the phone model they were made on | Correct readings on your phone, and warn when a profile came from another phone | On your phone |
| Settings: theme, weighting, threshold, language and similar choices | To remember your choices | On your phone |
| Crash reports and basic app events (Firebase, release builds only) | Fix crashes, understand general usage | Sent to Google Firebase (see 4) |

Decibly does not read your location, contacts, files, photos, messages, accounts or the list of your apps. Places are
text you type.

## 2. Permissions
- **Microphone** (`RECORD_AUDIO`) — for the meter, analyzer, logging sessions and mic check. Asked when you first start
  measuring, with an explanation. Sound is analysed in memory; apart from optional event clips (section 3) no audio is
  stored, and no audio is ever sent. You can refuse or turn it off in Android settings; stored sessions and reports
  stay readable.
- **Background logging and night watch** (`FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_MICROPHONE`) — optional. They
  start only when you tap Start logging in Background mode, "Keep logging with the screen off", or Arm night watch on the
  Monitor screen; never on their own, at boot or from the background. An ongoing notification shows the level and a
  Stop button while they run. For night watch the microphone turns on at your Arm tap, but sound before your chosen
  window is ignored: nothing is measured or saved until the window opens, and recording stops when it closes. The
  microphone is used exactly as in the app: levels in memory, no audio sent.
- **Notifications** (`POST_NOTIFICATIONS`, Android 13 and later) — asked only when you choose Background mode or night
  watch, to show that ongoing notification. If you refuse, logging still works and you stop it in the app.
- Normal permissions granted at install without a prompt: internet and network state (Firebase and Google Play) and
  advertising ID (Firebase Analytics). Libraries in the app may add related normal permissions (for example Android's
  ad-services permissions from the Google Mobile Ads SDK, or background-work permissions used by Android's WorkManager
  for widgets); they are not used to collect anything beyond what this policy describes.
- Decibly has **no location, camera or storage permission**: exports use Android's file picker and share sheet.

## 3. Event clips, exports, backups and feedback
**Event clips** are off by default. When you turn them on, each event above your threshold during a logging session
saves about 10 seconds of sound around it in the app's private storage on your phone. You can play or delete a clip in
Reports, and deleting a session deletes its clips. The app never uploads or shares clips. Turning the switch off stops
new clips; existing ones stay until you delete them.

**Exports and share cards:** when you export a session (PDF, CSV or JSON) or share a reading as an image card, the
file is created on your phone and saved only where you choose with Android's file picker, or sent with the app you
pick in the share sheet. A report contains the levels, events, the place and notes you typed, your phone model,
Android version and the calibration used; it goes only where you send it. Exports never contain audio.

**Backups and new phones:** Android's cloud backup (your Google account) includes only the app's settings, never your
sessions or clips. When you move to a new phone with Android's device-to-device transfer (cable or direct transfer,
Android 12 and later), your settings and sessions can be copied straight from your old phone to the new one; clips are
never copied, and that copy never goes through us. On Android 11 and lower, backups and transfers include only the
settings.

**Feedback:** when you use "Contact us", your e-mail app opens with the app version, Android version and phone model
added so we can help; you decide whether to send it.

## 4. Third-party services
The app includes Google components that follow Google's privacy policy (https://policies.google.com/privacy):

- **Firebase Crashlytics** (release builds) — crash and error reports: stack traces, device model, Android version,
  app version, free memory and disk at the time, and a Crashlytics installation ID. https://firebase.google.com/support/privacy
- **Firebase Analytics** (release builds) — automatically collected events (first open, sessions, screens viewed)
  with an app instance ID and the advertising ID. Your audio, clips, levels, sessions, places and notes are not sent.
- **Google Play in-app updates and in-app review** — to offer updates and, occasionally, a review prompt.
- **Google Play Billing** — included for a possible future one-time "Pro" purchase, but **not active in this version**:
  every feature is free and nothing can be bought.
- **Google AdMob and User Messaging Platform** — included for possible future ads, but **not active in this version**:
  no ads are shown and AdMob is never started. If ads or purchases are ever turned on, this policy will be updated
  first and the app will ask for consent where the law requires it. Audio will never be passed to ads.

## 5. Sharing and selling
We do not sell, rent or share personal data. Google processes the Firebase and Play data above as our service
provider.

## 6. Children
Decibly is not directed at children under 13, and we do not knowingly collect personal information from them.

## 7. Keeping and deleting data
Your sessions, clips, spots, calibration profiles and settings stay on your phone until you delete them. You can
delete a session (with its clips), a single clip or a spot in the app. A deleted session is hidden at once, can be
restored with Undo, and is removed for good, with its clips, the next time the app starts. You can remove everything by uninstalling the app or via Android
Settings › Apps › Decibly › Storage › Clear storage. Files you exported are not touched; delete them where you saved
or sent them. Firebase keeps crash reports for about 90 days and analytics data according to its retention settings.
To ask for deletion of crash or analytics data, write to tecdroiddeveloper@gmail.com. Deletion page:
https://adhavpavan.github.io/app-privacy-policy/decibly/delete-data/

## 8. Security
App data, including event clips, is kept in Android's private app storage. Connections to Google services are
encrypted (HTTPS). No audio, clip, level, session or place is sent anywhere by the app.

## 9. Changes
We may update this policy when the app changes. The current version, with its effective date, is always in the app
(menu › Privacy policy) and at https://adhavpavan.github.io/app-privacy-policy/decibly/.

## 10. Contact
Questions or requests about privacy: tecdroiddeveloper@gmail.com
