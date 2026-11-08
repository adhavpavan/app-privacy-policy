# Privacy Policy — QR Code Scanner & Generator

**Effective date:** 2026-11-08
**App:** QR Code Scanner & Generator (`com.techdev.qrscanner`) for Android
**Contact:** [tecdroiddeveloper@gmail.com](mailto:tecdroiddeveloper@gmail.com)

**In short:** what you scan and create stays on your phone. There is no account and no server of ours. Camera
frames are read in memory to find codes and are never saved or sent. Reading a code and checking a link work
fully offline: the app never looks up, fetches or follows a scanned link by itself. To fix crashes and understand
general usage, release builds use Google Firebase Crashlytics (crash reports) and Firebase Analytics (basic app
events such as app opens and screens viewed, with device identifiers including the advertising ID). These never
include your scans, history or codes. This version shows no ads. We never sell data.

## 1. What the app processes, and where
All processing happens on your phone. What the app stores is kept in its private storage (a local database, its
settings and a folder for logos you add to codes), which other apps cannot read.

| Information | Why | Where it stays |
|---|---|---|
| Camera frames (only after you allow the camera) | To find and read codes while the Scan tab is open | Processed in memory and thrown away. **Never saved, recorded or sent** |
| A picture you pick to scan (Android photo picker, or an image shared to the app) | To read the codes in it | Read once on your phone; the picture is not copied or kept |
| Scan history: the code's content, type, time, source (camera, picture, batch), the link check result, your notes and favourites | History, search, batch lists | On your phone until you delete it, or auto-delete removes it (Settings) |
| Codes you create (My codes): their content, label, design and any logo picture you choose | My codes, Show mode, the My code widget | On your phone; a logo is copied into the app's private storage |
| Wallet cards: name, card number, barcode type, colour, tags, note | Wallet › Cards, Show at the till | On your phone, in the app's private database |
| My card: the contact code you choose as My card | Home, Show mode, the My card widget | On your phone (it is one of your My codes) |
| A PDF you pick to scan (Android file picker) | To read the code on the page you choose | Read page by page on your phone; the file is not copied or kept |
| 2-step verification setup codes (`otpauth://`) | To hand them to your authenticator app | **Never saved to history**; screenshots are blocked while one is shown |
| Link check (offline) | To show what a scanned link really points to and warn about common tricks | Done on your phone with lists built into the app; nothing is looked up online |
| Clipboard | Only when you tap "From clipboard" / paste, to fill a form or the link checker | Read once on your phone, never stored or sent by itself |
| Settings: theme, language, sounds, history options | To remember your choices | On your phone |
| Crash reports and basic app events (release builds) | Fix crashes, understand general usage | Sent to Google Firebase (see 4) |

The app does not read your location, contacts, files, messages, accounts, saved Wi-Fi networks or the list of your
apps. Adding a contact or calendar event from a scan opens Android's own screen, where you decide.

## 2. Permissions and how they are used
### Camera (`CAMERA`)
To scan codes. Asked on the welcome screen when you tap Allow, or when you first open the Scan tab. Frames are read
in memory only. The camera is optional: you can scan from pictures instead, and turn the permission off any time in
Android settings.

### Wi-Fi (`ACCESS_WIFI_STATE`, `CHANGE_WIFI_STATE`)
Only when you tap "Join" on a scanned Wi-Fi code, to hand that network to Android. Depending on the Android
version, Android shows its own "Save network?" sheet or a suggestion notification and you decide. The app does not
read or list your saved networks.

### Internet and network state (`INTERNET`, `ACCESS_NETWORK_STATE`)
Used only by Firebase Crashlytics, Firebase Analytics and Google Play services (updates, review, purchases).
Scanning, the link checker and code creation never use the network. Opening a link or searching the web happens only
when you tap that action, and then your browser or the website handles it under its own policy.

### Advertising ID (`AD_ID`)
Read by Firebase Analytics (release builds). No ads are shown in this version.

### Fingerprint, face or screen lock (`USE_BIOMETRIC`, `USE_FINGERPRINT`)
Only if you turn on Wallet › Cards › Lock cards. Android shows its own fingerprint, face or screen-lock prompt and tells
the app only whether it worked. The app never sees, stores or sends biometric data. Added by Android's biometric
library; nothing is asked until you turn the lock on.

### Vibration (`VIBRATE`)
Short haptic feedback when a code is read or a button is pressed. You can turn haptics off in Settings.

## 3. Exports, backups, restore, widget and feedback
- **Exports and sharing.** When you share a result, export history (CSV or JSON), make a full backup or save a code as
  an image, PDF or SVG, the file is created on your phone and saved only where you choose with Android's file picker,
  or sent with the app you pick in the share sheet. If the file would include Wi-Fi codes, the app asks first whether
  it may contain their passwords.
- **Restore.** Restoring a backup reads only the file you pick and adds its contents to the app. Nothing is sent
  anywhere.
- **Widgets.** The Scan widget opens the scanner. The My code widget shows a code you chose on your home screen, so
  anyone who can see your home screen can see and scan it. Widget data stays on your phone; remove the widget to
  hide it.
- **Android backup.** Android may include the app's database (history and My codes), settings and logo pictures in
  your own device backup (for example your Google account backup) or a phone-to-phone transfer, if you turned that
  on. Android and Google manage and encrypt it; we cannot read it.
- **Feedback.** "Contact us" opens your e-mail app with the app version, Android version and phone model added so we
  can help. You decide whether to send it.

## 4. Third-party services
Release builds include Google components that follow Google's privacy policy
(<https://policies.google.com/privacy>):
- **Firebase Crashlytics** — crash and error reports: stack traces, device model, Android version, app version, app
  state at the time, and a Crashlytics installation ID. <https://firebase.google.com/support/privacy>
- **Firebase Analytics** — automatically collected events (first open, sessions, screens viewed) with an app instance
  ID and the advertising ID. The content of your scans, history and codes is never sent.
- **Google ML Kit barcode scanning** — reads codes on your phone with a model bundled in the app.
- **Google Play in-app updates and in-app review** — to offer updates and, now and then, a review prompt.
- **Google Play Billing** — if Pro is offered, Google handles the payment; the app only learns whether Pro is owned by
  your Google account.
- **Google AdMob** — included for possible future ads but **turned off**: no ads are shown and AdMob is never
  started. If ads are ever turned on, this policy will be updated first and the app will ask for consent where the
  law requires it.

## 5. Sharing and selling
We do not sell, rent or share personal data. Google processes the Firebase and Play data above as our service
provider.

## 6. Children
The app is not directed at children under 13, and we do not knowingly collect personal information from them.

## 7. Keeping and deleting your data
History and My codes stay on your phone until you delete them. You can delete single scans, clear all history in
Settings, or set history to auto-delete after 30 or 90 days. Uninstalling the app, or Android Settings › Apps ›
QR Code Scanner & Generator › Storage › Clear storage, removes everything on the phone. Files you exported are not
touched; delete them where you saved them. Firebase keeps crash reports for about 90 days and analytics data
according to its retention settings. To ask for deletion of crash or analytics data, write to
[tecdroiddeveloper@gmail.com](mailto:tecdroiddeveloper@gmail.com) with the app instance ID shown in the app's About
screen. Deletion page: <https://adhavpavan.github.io/app-privacy-policy/qr-scanner/delete-data/>

## 8. Security
App data is kept in Android's private app storage, which other apps cannot read. Connections to Google services
are encrypted (HTTPS). No camera image, scan or code is sent anywhere by the app.

## 9. Changes to this policy
We may update this policy when the app changes. The current version, with its effective date, is always in the app
(menu › Privacy policy) and at <https://adhavpavan.github.io/app-privacy-policy/qr-scanner/>.

## 10. Contact
Questions or requests about privacy: [tecdroiddeveloper@gmail.com](mailto:tecdroiddeveloper@gmail.com)
