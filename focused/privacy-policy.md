# Privacy Policy — Focused: Screen Time Control

**Effective date:** 19 November 2026
**App:** Focused: Screen Time Control (`com.techdev.focused`) for Android phones and tablets, and for Android TV
**Contact:** [tecdroiddeveloper@gmail.com](mailto:tecdroiddeveloper@gmail.com)

This policy explains how Focused: Screen Time Control ("Focused", "the app", "we") handles information. It covers
the phone app and the Android TV app (same package name). Sections 1 to 9 describe the phone app; section 10
describes how the TV app differs.

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
| Your rules: app limits, schedules, focus sessions and presets (including Whole-phone focus, which blocks every app except the ones you keep), strict mode, website rules, programs, goals | To enforce what you set | On your phone |
| Content filter settings, if you use it: whether the adult filter is on and your list of blocked words | To block matching pages | On your phone |
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
- if you turn on the optional **content filter**, the same address-bar text (including search words a browser shows
  there) is also checked, on your phone, against the list of adult sites built into the app and your own blocked words.
  When a page matches, only the fact that it was blocked is stored (as for websites); the address and the matching word
  are never stored or sent.
- the **list of open windows**, only to find a **picture-in-picture** window and its app's package name, so a blocked
  app can't keep playing in a floating window.

The service does **not** read any other text on your screen, never records what you type, passwords or messages, and
its only actions are going **Back** or **Home** to leave a blocked app and closing a blocked app's picture-in-picture
window. Nothing it sees leaves your phone. You can turn
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
- **Share cards:** if you share an achievement from the Achievements screen, the app draws an image on your phone (the
  achievement, your streak, average focus score and badge count, no other usage details) and hands it to the app you
  pick in Android's share sheet. We never receive it.
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
- **Google Play Billing** — for the optional "Remove ads" purchase when it is offered, and the optional paid early
  exit (a one-time purchase that ends a strict or Deep focus session, or lifts a strict limit until midnight). The
  purchase carries only an internal number of that session or limit (never its name or apps), so the app can end the
  right one. We never see your payment details; Google Play only tells the app whether a purchase was made.
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
the app (phone: Me → Privacy policy; TV: Settings → Privacy policy) and on this page.

## 10. Focused for Android TV

The TV app follows the same rules as the phone app: everything it measures stays **on the TV**, there are no accounts and no servers of ours, and nothing is sold. Where it differs:

**What it processes and stores on the TV** (in the app's private storage, which other apps cannot read):

| Information | Why |
|---|---|
| Watch time per app, per day and per hour | Today screen, insights, daily allowance and app limits |
| Your rules: app limits, schedules (such as bedtime), the daily TV allowance, watch breaks, timers, always-allowed apps and settings | To enforce what you set |
| Time's-up events (when the block screen appeared, for which app and why, and what happened next) | Insights and the parent's history |
| Extra time granted with the parent PIN, until it ends | To let a granted app run until then |
| The parent PIN, as a salted hash only (never the PIN as typed) | To check the PIN; the hash cannot be turned back into the PIN |
| An optional PIN hint, as the parent typed it (it may not contain the PIN) | Shown on "Forgot PIN?" to help the parent remember |
| The PIN recovery code, as a salted hash only (the code is shown once and never stored) | To reset a forgotten PIN |
| The time a requested 48-hour PIN reset will happen, if one was started | To show the countdown and remove the PIN when it ends |
| Whether Focused Pro is active (yes/no) | So Pro features keep working without a network connection |

Watch history older than about 13 months and time's-up events older than about 4 months are deleted automatically.

**Usage access (`PACKAGE_USAGE_STATS`), optional.** If you allow it, the TV app reads from Android how long each app was used, to include watching from before Focused was set up. Many TVs hide this setting; the app then measures watch time itself (below). The data stays on the TV.

**Accessibility service ("guard"), needed for limits.** Turned on only after an in-app explanation. On the TV it sees **only which app is on the screen** (the package name of the active window), to count watch time and to show the time's-up, bedtime or PIN screen. It does **not** read any text, titles, subtitles, search words, voice input or anything you type, does not look at web addresses or short videos, and does not record the screen. Its only actions are going to the TV **Home** screen and, if you choose "sleep the TV" when a timer ends, asking Android to lock or sleep the screen. Nothing it sees leaves the TV. You can turn it off in the TV's Settings → Accessibility.

**Focused Pro subscription (Google Play Billing), optional.** Focused Pro is an auto-renewing subscription (every 3 months or every year, sometimes with a free trial for new subscribers) bought through **Google Play**. Google Play handles the payment and your payment details; we never see them. Google Play tells the app only whether the subscription is active, and the app keeps that yes/no on the TV. Purchases are linked to your Google account by Google, not by us. You can cancel at any time in Google Play → Payments & subscriptions → Subscriptions; Pro then ends when the paid period ends. Google's handling of the purchase is covered by the [Google Payments privacy notice](https://payments.google.com/payments/apis-secure/get_legal_document?ldo=0&ldt=privacynotice). Release versions' Firebase Analytics may record an automatic in-app purchase event (product and price; never your watch time, apps, rules or PIN), as described in section 4.

**Start at boot (`RECEIVE_BOOT_COMPLETED`).** Used only to restore your rules after the TV restarts or the app updates.

**Not in the TV app:** no ads or AdMob SDK, no one-time purchases (only the Focused Pro subscription above), no in-app review or update prompts, no notifications, no backups or CSV exports, no share cards, no website rules or content filter, no location.

**Network and third parties.** Release versions use the same **Firebase Crashlytics** and **Firebase Analytics** described in section 4, with the same data (including the advertising ID for Analytics, declared with the `AD_ID` permission) and the same retention. They never receive your watch time, app names, rules or PIN.

**Android device backup.** As on the phone, if Android's own backup is on, the TV may include the app's data in your encrypted Google account backup. This is managed by Android and Google, not by us.

**Children and family mode.** In family mode a parent sets Focused up on the TV. A child's watch time is shown only on that TV and is never sent to us or anyone else. Section 6 applies to the TV app too.

**Deleting your data on the TV.** Clear the app's data (TV Settings → Apps → Focused → Clear data) or uninstall the app. Everything it stored is removed; nothing is kept on a server.

## 11. Contact

Questions or requests about privacy? Write to
[tecdroiddeveloper@gmail.com](mailto:tecdroiddeveloper@gmail.com).
