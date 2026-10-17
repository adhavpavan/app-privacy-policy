# Privacy Policy — Focused: Screen Time Control

**Effective date:** 17 October 2026
**App:** Focused: Screen Time Control (`com.techdev.focused`) for Android
**Contact:** [tecdroiddeveloper@gmail.com](mailto:tecdroiddeveloper@gmail.com)

This policy explains how Focused: Screen Time Control ("Focused", "the app", "we") handles information.

**In short:** your usage data stays on your phone. Your usage statistics, the names of the apps you use, the
websites you visit, your rules and anything the accessibility service sees are never sent anywhere. There are no
accounts and no servers of ours. To fix crashes and understand how the app is used in general, the app uses Google
Firebase Crashlytics (crash reports) and Firebase Analytics (basic app events such as app opens and screens viewed,
with device identifiers including the advertising ID). We never sell your data, and we never receive your usage data.

---

## 1. What the app processes, and where

All processing happens **on your device**. The results are stored only in the app's private storage (its local
database and settings), which other apps cannot read.

| Information | Why | Where it stays |
|---|---|---|
| App usage statistics from Android (apps used and for how long, app opens, phone unlocks, number of notifications per app) | Screen time, sessions, pickups, focus score, goals, history, limits | On your phone |
| Your rules: app limits, schedules, focus sessions and presets, strict mode, website rules, goals | To enforce what you set | On your phone |
| Domains of your own website rules and the time spent on them | Website limits and blocking | On your phone |
| Optional display name on the Me tab | Personalisation | On your phone |

We do **not** collect your name, e-mail address, phone number, contacts, messages, photos, files or browsing history.
The only information sent off your phone is the crash and analytics data described in section 4.

## 2. Permissions and how they are used

### Usage access (`PACKAGE_USAGE_STATS`)
Android lets the app read the phone's own usage statistics: which apps you used and for how long, app opens, unlocks
and how many notifications each app posted. This is the core of the app. The content of notifications is never read;
they are only counted from Android's usage statistics.

### Accessibility service ("Focused blocking")
Optional, and only active if you turn it on after an in-app explanation. It is used **only** to enforce the limits,
schedules and blocks you set. It looks at:

- the **app in the foreground** and the name of its current screen (window class), to show the block screen;
- in supported **short-video apps** (such as Instagram Reels and YouTube Shorts), **known screen element IDs**, to
  recognise and count short videos;
- in supported **browsers**, **only the address bar**, to match the websites you chose to block or limit. It is not read
  while you are typing in it. Only the domains of your own rules and the time spent are stored.

The service does **not** read any other text on your screen, never records what you type, passwords or messages, and
its only actions are going **Back** or **Home** to leave a blocked app. Nothing it sees leaves your phone. You can turn
it off at any time in Android Settings → Accessibility.

### Location
Focused does **not** ask for or use your location.

### Do Not Disturb access (optional)
Used only to silence notifications during focus sessions if you turn on that option. Your previous setting is restored
when the session ends.

### Notifications
Used to show reminders, limit warnings, the focus timer, daily and weekly summaries, and other alerts you turn on.

### Internet and network state
The app has no server of its own. Network access exists only for the Google components listed in section 4,
including sending crash reports through Firebase Crashlytics and basic app events through Firebase Analytics.

### Advertising ID (`AD_ID`)
The advertising ID is a resettable identifier that Google Play services provides on Android. Focused declares the
advertising ID permission because Firebase Analytics collects it, together with the app instance ID, to measure how
the app is used. Ads are currently turned off, so it is not used to show ads; if a future version shows ads, Google
AdMob will also use it (see section 4). You can reset or delete your advertising ID, or opt out of ads
personalisation, at any time in your phone's settings (for example Settings → Google → Ads, or Settings → Privacy →
Ads, depending on your phone). After you delete it, apps no longer receive an advertising ID.

## 3. Backups, exports and feedback

- **Backups and CSV exports** are created only when you ask for them and are saved to the location you pick in Android's
  file picker (for example your phone storage or a cloud drive of your choice). We never receive these files. They
  contain your usage history and rules, so keep them somewhere safe.
- **Android device backup:** if Android's own backup is turned on, Android may include the app's database and settings
  in your encrypted Google account backup so they can be restored on a new phone. This is managed by Android and Google,
  not by us, and can be turned off in your phone's settings.
- **Feedback:** if you use *Contact us*, your e-mail app opens with our address, a subject with the app version and, in
  the message, the app version, Android version and phone model to help us answer. You can remove them before sending.
  We use your e-mail only to reply to you.

## 4. Third-party services

The app includes these Google components, which are governed by
[Google's Privacy Policy](https://policies.google.com/privacy):

- **Google Play In-App Review and In-App Updates** — to rate the app and install updates.
- **Firebase Crashlytics** — if the app crashes or hits a serious error, a crash report is sent to Google (Firebase),
  acting as our service provider. It contains the error and stack trace, the device model, Android version, app
  version, the device state at the time of the crash (such as free memory and disk space, and screen orientation) and
  a random Crashlytics installation ID (not the advertising ID). It contains no usage data, rules or personal content.
  It is sent encrypted, used only to find and fix crashes, never used for ads and never sold. Firebase keeps crash
  data for about 90 days. See [Firebase privacy and security](https://firebase.google.com/support/privacy).
- **Firebase Analytics (Google Analytics for Firebase)** — to understand how the app is used in general (for example
  how many people open it, which screens are viewed and which app versions are in use), so we can improve it. The app
  logs no events of its own; Firebase Analytics records only its
  [automatically collected events](https://support.google.com/firebase/answer/9234069), such as first open, session
  start, screen views, app updates, Android updates and in-app purchases. With them it collects the app instance ID,
  the advertising ID, device model, Android version, language, app version, approximate country or region (derived
  from your IP address) and engagement time. It never receives your usage statistics, the names of the apps you use,
  websites, rules or anything the accessibility service sees. Data is sent encrypted to Google (Firebase), acting as
  our service provider, is not sold, and is kept by Google for a limited time, as configured in Firebase (by default
  2 months for user-level data). See [Firebase privacy and security](https://firebase.google.com/support/privacy).
- **Google Play Billing** — for the optional "Remove ads" purchase when it is offered. We never see your payment
  details; Google Play only tells the app whether the purchase is owned.
- **Google AdMob and the User Messaging Platform (UMP)** — **ads are currently turned off** and no ads are requested.
  If a future version shows ads, you will be asked for consent where the law requires it (for example in the EEA, the
  UK and some US states) and can change your choice in the app. AdMob may then collect device identifiers such as the
  advertising ID, as described in
  [How Google uses information from sites or apps that use its services](https://policies.google.com/technologies/partner-sites)
  and [Google's advertising policy](https://policies.google.com/technologies/ads). You can reset or delete your
  advertising ID in your phone's settings.

Firebase Analytics is the only analytics SDK in the app. The AdMob SDK is included but stays inactive while ads are
turned off. None of these services receive your usage data.

## 5. Sharing and selling

We do not sell or rent your information, and we do not share it with third parties for their own purposes. Your usage
data is never sent to us or to anyone else. Crash reports and analytics data are processed by Google (Firebase) as our
service provider, only to help us fix crashes and understand how the app is used.

## 6. Children

Focused is not directed at children under 13, and we do not knowingly collect personal information from children.
Because the app sends no usage data to us, we hold no such information.

## 7. Keeping and deleting your data

Your data stays on your phone until you delete it. You can:

- reset the app's statistics archive in **Settings → Reset statistics archive**;
- delete individual limits, schedules, or website rules;
- remove everything by clearing the app's storage (Android Settings → Apps → Focused → Storage → Clear storage) or by
  uninstalling the app.

The usage statistics themselves are kept by Android (not by Focused) according to Android's own rules. Backup files
you saved elsewhere are yours to delete. We store none of your usage data, so there is nothing for us to delete
on a server. Crash reports are deleted automatically by Firebase after about 90 days. Analytics data is kept by Google
for a limited time, as configured in Firebase (by default 2 months for user-level data). You can also reset or delete
your advertising ID in your phone's settings. To ask for earlier deletion, write to
[tecdroiddeveloper@gmail.com](mailto:tecdroiddeveloper@gmail.com).

## 8. Security

Your usage data is kept in the app's private storage, which other apps cannot read, and the app does not send it over
the internet. Crash reports and analytics data are sent to Firebase over an encrypted (HTTPS) connection. Protect your phone with a screen
lock and keep backup files somewhere safe.

## 9. Changes to this policy

We may update this policy when the app changes. The current version, with its effective date, is always available in
the app (Me → Privacy policy) and on this page.

## 10. Contact

Questions or requests about privacy? Write to
[tecdroiddeveloper@gmail.com](mailto:tecdroiddeveloper@gmail.com).
