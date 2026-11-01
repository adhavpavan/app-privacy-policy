# Privacy Policy — Data Manager and App Usage

Effective date: 1 November 2026 · Package `com.techdev.internetspeedmeter` · Contact: techdevpavan@gmail.com

**In short:** Data Manager and App Usage reads your screen time, app usage and data usage from Android's own
statistics and keeps them on your phone. There is no account and no server of ours, and this usage data is never
uploaded. To fix crashes and understand how the app is used in general, the app uses Google Firebase Crashlytics
(crash reports) and Firebase Analytics (app interactions such as app opens and screens viewed). The free version may
show native ads from Google AdMob, with a consent form where the law requires one. "Remove ads" is bought through
Google Play. We never sell data.

## 1. What the app processes, and where
All usage processing happens on your device. What the app stores is kept in its private storage (local database and
settings), which other apps cannot read.

| Information | Why | Where it stays |
|---|---|---|
| Screen time, app launches, notification counts, unlocks and sessions (Android usage statistics) | Time tab, Home, App details, insights, limits and alerts | On your phone |
| Data usage per app and in total, Wi-Fi / mobile, roaming and hotspot (Android network statistics) | Data tab, plans, alerts, widgets | On your phone |
| Live network speed, from the phone's own traffic counters | Status-bar speed meter, Quick Settings tile | In memory; on your phone. No speed test data is sent to any server |
| List of installed apps with names, icons, versions, permissions and storage size | To name the apps in your usage, App details | On your phone |
| Your data plans, limits, alert rules, goals, activity feed and settings | To remember your choices and run alerts | On your phone |
| Crash reports and app interactions (Firebase, release builds only) | Fix crashes, understand general usage | Sent to Google Firebase (see 4) |

If Android backup is on, Android may include the app's history, plans and settings in your phone's backup to your
Google account, and moves them to a new phone. Android manages that backup; we cannot read it.

## 2. Permissions
- **Usage Access** (special access you grant in Android Settings) — to read screen time, app launches,
  notifications, unlocks and per-app data usage.
- **Phone** (Android 7–9 only) — Android requires it to read mobile data totals per SIM. The app never makes calls
  and never reads your phone number.
- **Notifications** — for the speed meter, alerts and summaries you turn on.
- **Foreground service and run at startup** — keep the status-bar speed meter running while you have it on, and
  restart it and the scheduled checks after the phone restarts.
- **Biometrics** — only for App lock, if you turn it on. Android checks your fingerprint, face or screen lock; the
  app never sees them.
- **Request uninstall** — only when you tap Uninstall in App details; Android asks you to confirm.
- **Internet and network state** — for Firebase, ads and consent, and Google Play (purchases, updates, reviews).
- **Advertising ID** — used by AdMob and Firebase Analytics.
- **Google Play billing** — for the "Remove ads" purchase.

## 3. Exports, backups and feedback
Reports, backup files and data files you export are created on your phone and go only where you save or share them
(for example a folder or Google Drive you choose). When you use "Contact us" or send feedback, your e-mail app opens
with the app version, Android version and phone model added so we can help.

## 4. Third-party services
The app includes Google components that follow Google's privacy policy (https://policies.google.com/privacy):

- **Firebase Analytics** (release builds) — app interactions collected automatically: first open, sessions, screens
  viewed, in-app purchases and app updates, with device model, Android version, language, approximate country (from
  the IP address), an app instance ID and the advertising ID. No usage numbers, app names or package names are
  logged, and the app logs no custom events. Google consent mode is on: where the law requires consent, Analytics
  follows your choice in the consent form.
- **Firebase Crashlytics** (release builds) — crash reports and diagnostics: stack traces, device model, Android
  version, app version, free memory and disk space at the time, and a Crashlytics installation ID.
  https://firebase.google.com/support/privacy
- **Firebase Remote Config** — downloads app settings, such as whether ads are on.
- **Google AdMob and User Messaging Platform** — when ads are on, the free version shows native ad cards inside the
  app's screens, each marked "Ad". There are no banner or full-screen ads. Where the law requires it (for example in
  the EEA, the UK, Switzerland and some US states), the consent form asks for your choice before any ad is
  requested; you can change it at any time in Settings → Privacy options. AdMob may use cookies, the advertising ID,
  your IP address (approximate location) and your interactions with ads to show, personalise and measure ads.
  https://policies.google.com/technologies/ads
- **Google Play Billing** — the one-time "Remove ads" purchase. Google handles payment; the app only learns whether
  your Google account owns it. Owners never see ads.
- **Google Play in-app updates and in-app review** — to offer updates and, now and then, a rating prompt.

## 5. Sharing and selling
We do not sell, rent or share personal data. Google processes the Firebase, AdMob and Play data above under its own
policies.

## 6. Children
The app is not directed at children under 13, and we do not knowingly collect personal information from them.

## 7. Keeping and deleting data
Data stored by the app stays on your phone until you delete it: Settings → Clear All Data in the app, clearing the
app's storage in Android Settings, or uninstalling the app removes all of it. Firebase keeps crash reports for 90 days
and analytics data for up to 14 months. You can reset or delete your advertising ID in your phone's settings. There
is no account; to ask for deletion of crash or analytics data, write to techdevpavan@gmail.com. Deletion page:
https://adhavpavan.github.io/app-privacy-policy/data-manager/delete-data/

## 8. Security
App data is kept in Android's private app storage. Connections to Google services are encrypted (HTTPS).

## 9. Changes
We may update this policy when the app changes. The current version, with its effective date, is always in the app
(Settings → Privacy Policy) and at https://adhavpavan.github.io/app-privacy-policy/data-manager/.

## 10. Contact
Questions or requests about privacy: techdevpavan@gmail.com
