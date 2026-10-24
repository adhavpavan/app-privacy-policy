# Privacy Policy — Northwise: Digital Compass

Effective date: 25 October 2026 · Package `com.techdev.northwise` · Contact: tecdroiddeveloper@gmail.com

**In short:** Northwise shows your heading, the sun and the moon, and keeps what you save on your phone. There is no
account and no server of ours. Location is optional: it is asked only when you tap "Use my location", used only while
the app is open, never in the background, and never sent anywhere. Camera pictures are only shown on screen to aim and
are never saved or sent. To fix crashes and understand how the app is used in general, it uses Google Firebase
Crashlytics (crash reports) and Firebase Analytics (basic app events such as app opens and screens viewed, with device
identifiers including the advertising ID). This version shows no ads and sells nothing. We never sell data.

## 1. What the app processes, and where
All processing happens on your device. What the app stores is kept only in its private storage (a local database and
settings), which other apps cannot read.

| Information | Why | Where it stays |
|---|---|---|
| Sensor readings: magnetic field, accelerometer, gyroscope and the orientation Android works out from them | Heading, tilt, level bubble, accuracy ring, calibration coach, camera sight | Processed on your phone while a compass screen is open; the coach keeps your last check results on the phone |
| Your position for true north and sun times: a city from the list built into the app, coordinates you type, or a fix from your phone's location if you choose "Use my location" | Magnetic declination (true north), sun and moon times and directions, direction and distance to a place | On your phone. A position from your location is kept only when you save it |
| Live location (only after you tap "Use my location" and allow it): coordinates, accuracy, GPS altitude, speed and satellites | The live position card and a live "Here" in Point to a place | In memory while that screen is open. **Never sent anywhere** |
| Camera preview (only after you open the camera sight and allow the camera) | To show what you aim at | Shown on screen only. **Never captured, saved or sent** |
| Saved bearings and places: the names, notes, bearings, elevations and coordinates you save | Bearings tab, widgets, Point to a place | On your phone until you delete them or uninstall |
| Settings: north reference, units, coordinate format, theme, night mode, language | To remember your choices | On your phone |
| Crash reports and basic app events (Firebase, release builds only) | Fix crashes, understand general usage | Sent to Google Firebase (see 4) |

Northwise does not read your contacts, files, photos, messages, microphone, accounts or the list of your apps, and it
never uses your location in the background.

## 2. Permissions
- **Location** (`ACCESS_FINE_LOCATION`, `ACCESS_COARSE_LOCATION`) — optional. Asked only when you tap "Use my
  location", after a short explanation. It is used only while you use the app, never in the background: to set your
  position for true north and sun times, to show live coordinates, altitude and speed, and to keep "Here" current in
  Point to a place. You may allow only approximate location. Your location is never sent anywhere. If you refuse, the
  app works fully with a city or typed coordinates; you can turn the permission off at any time in Android settings.
- **Camera** (`CAMERA`) — only for the camera sight in the Sight tab. Asked only when you turn the camera on. The
  picture is shown on screen to aim and is never saved or sent. If you refuse, the sighting tape works without it.
- Normal permissions granted at install without a prompt: internet and network state (Firebase and Google Play) and
  advertising ID (Firebase Analytics). Libraries in the app may add related normal permissions (for example Android's
  ad-services permissions from the Google Mobile Ads SDK, the Play install referrer used by Firebase Analytics, or
  background-work permissions used by Android's WorkManager to refresh widgets); they are not used to collect anything
  beyond what this policy describes.
- Northwise has **no microphone permission, no background location and no access to your storage**.

## 3. Sharing, backups and feedback
When you share a bearing as an image card, the image is created on your phone and sent only with the app you pick in
the share sheet; it shows the bearing's name, bearing, back-bearing and north reference, not your position. Android
may include the app's settings, saved position, bearings and places in your own Google account backup if you turned
device backup on; that is handled by Android and Google, not by us. When you use "Contact us", your e-mail app opens
with the app version, Android version and phone model added so we can help; you decide whether to send it.

## 4. Third-party services
The app includes Google components that follow Google's privacy policy (https://policies.google.com/privacy):

- **Firebase Crashlytics** (release builds) — crash and error reports: stack traces, device model, Android version,
  app version, free memory and disk at the time, and a Crashlytics installation ID. https://firebase.google.com/support/privacy
- **Firebase Analytics** (release builds) — automatically collected events (first open, sessions, screens viewed)
  with an app instance ID and the advertising ID. Your position, location, bearings, places and camera pictures are
  not sent.
- **Google Play in-app updates and in-app review** — to offer updates and, occasionally, a review prompt.
- **Google Play Billing** — included for a possible future one-time "Pro" purchase, but **not active in this version**:
  every feature is free and nothing can be bought.
- **Google AdMob and User Messaging Platform** — included for possible future ads, but **not active in this version**:
  no ads are shown and AdMob is never started. If ads or purchases are ever turned on, this policy will be updated
  first and the app will ask for consent where the law requires it. Your location will never be passed to ads.

## 5. Sharing and selling
We do not sell, rent or share personal data. Google processes the Firebase and Play data above as our service
provider.

## 6. Children
Northwise is not directed at children under 13, and we do not knowingly collect personal information from them.

## 7. Keeping and deleting data
Your saved position, bearings, places and settings stay on your phone until you delete them. You can delete bearings
and places in the app and remove the saved position on the Position screen, or remove everything by uninstalling the
app or via Android Settings › Apps › Northwise › Storage › Clear storage. Images you shared are not touched; delete
them where you sent them. Firebase keeps crash reports for about 90 days and analytics data according to its retention
settings. To ask for deletion of crash or analytics data, write to tecdroiddeveloper@gmail.com. Deletion page:
https://adhavpavan.github.io/app-privacy-policy/northwise/delete-data/

## 8. Security
App data is kept in Android's private app storage. Connections to Google services are encrypted (HTTPS). No
location, camera picture, bearing or place is sent anywhere by the app.

## 9. Changes
We may update this policy when the app changes. The current version, with its effective date, is always in the app
(menu › Privacy policy) and at https://adhavpavan.github.io/app-privacy-policy/northwise/.

## 10. Contact
Questions or requests about privacy: tecdroiddeveloper@gmail.com
