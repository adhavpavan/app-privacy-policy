# Privacy Policy — WiFi Analyzer & Who's on WiFi

Effective date: 1 November 2026 · Package `com.techdev.wifianalyzer` · Contact: tecdroiddeveloper@gmail.com

**In short:** WiFi Analyzer is made by TechDev. There is no account and no server of ours, and nothing about your network is uploaded. Device names, your labels, scans, room checks and saved Wake-on-LAN targets stay on this phone. Android requires location permission before an app may see Wi-Fi names; the app never reads your position, never stores it and never uses location in the background. To fix crashes and understand general usage, release builds use Google Firebase Crashlytics and Firebase Analytics. Those reports never include network names, IP or hardware addresses, or device names, and you can turn analytics off in Settings. We never sell data.

## 1. What the app processes, and where
All processing happens on your device. What the app stores is kept only in its private storage, which other apps cannot read.

| Information | Why | Where it stays |
|---|---|---|
| Devices on your own Wi-Fi: addresses, names, services and open ports | A scan you start, or an optional new-device check you turned on | On your phone. Never uploaded |
| Connection details (signal, speed, router address) and nearby Wi-Fi network names | Signal and network screens | On your phone. Network names are not sent to us |
| Your labels, room checks and saved Wake-on-LAN targets | So the app remembers what you marked | On your phone until you delete them or uninstall |
| Addresses you type into ping, traceroute, port scan or DNS lookup | The tool you started | The app contacts only that address. Results stay on your phone |
| Optional vendor-list update | To name the maker of a hardware address | A one-time download of the public IEEE list. Your scans are not sent with it |
| Router page, if you open it | To show your router's own page | Loaded only from an address on your local network. Cookies and page storage are cleared when you leave. Passwords you type there are not sent to us |
| Crash reports and basic app events (Firebase, release builds) | Fix crashes, understand general usage | Sent to Google Firebase (see 4). Never includes network names, IP or hardware addresses, or device names |

The app does not read your contacts, files, photos, messages, accounts or the full list of installed apps. To offer a shortcut into a known router app, it checks only a short list of those apps.

## 2. Permissions
- **Location** (`ACCESS_FINE_LOCATION`, `ACCESS_COARSE_LOCATION`) — Android requires this before any app may see Wi-Fi network names or nearby networks. Asked only when you open a screen that needs it. The app never reads your position, never stores it and never uses location in the background. There is no background-location permission.
- **Nearby Wi-Fi devices** (`NEARBY_WIFI_DEVICES`, Android 13 and later, declared `neverForLocation`) — to reach devices on your Wi-Fi when Android limits local-network access. Not used for location.
- **Wi-Fi and network** (`ACCESS_WIFI_STATE`, `CHANGE_WIFI_STATE`, `ACCESS_NETWORK_STATE`, `CHANGE_WIFI_MULTICAST_STATE`, `INTERNET`) — to read the connection, request a scan, discover devices with multicast (mDNS and UPnP), and run a tool you start. Internet is also used for Firebase, Google Play and the optional vendor-list download.
- **Notifications** (`POST_NOTIFICATIONS`, Android 13 and later) — asked only when you turn new-device alerts on. If you refuse, the rest of the app keeps working.
- **New-device alerts** — off until you turn them on. The app then checks your home Wi-Fi every 15, 30 or 60 minutes (your choice) with Android's WorkManager, on Wi-Fi and when the battery is not low, and can notify you. There is no always-on foreground service and no background location. Turn alerts off in Settings to stop the checks.
- **Advertising ID** — used by Firebase Analytics in release builds. You can turn analytics off in Settings.
- The app does not request access to your storage. Exports use Android's file picker.

## 3. Exports, backups and sharing
Exports (CSV or JSON) and backups are created only when you ask, and saved or shared only where you choose. Nothing is shared automatically. Android may include the app's database and settings in your own Google account backup if you turned device backup on; that is handled by Android and Google, not by us. When you use Contact us, your e-mail app opens with the app version, Android version and phone model added so we can help; you decide whether to send it.

## 4. Third-party services
Release builds include Google components that follow Google's privacy policy (https://policies.google.com/privacy):

- **Firebase Crashlytics** — crash and error reports: stack traces, device model, Android version, app version and a Crashlytics installation ID. https://firebase.google.com/support/privacy
- **Firebase Analytics** — basic usage events such as app opens and screens viewed, with an app instance ID and the advertising ID. You can turn this off in Settings. Network names, IP or hardware addresses and device names are not sent.
- **Google Play in-app updates and in-app review** — to offer updates and, occasionally, a review prompt.
- **Google Play Billing** — for a Pro purchase, if offered. Google handles the payment; the app only learns whether Pro is owned by your Google account.
- **Google AdMob** — included for possible future ads, but not active in this version: no ads are shown and AdMob is never started. If ads are ever turned on, this policy will be updated first and the app will ask for consent where the law requires it.

## 5. Purchases
Pro, if offered, is bought through Google Play Billing. Google handles the payment. The app only learns whether Pro is owned by your Google account.

## 6. Sharing and selling
We do not sell, rent or share personal data. Google processes the Firebase and Play data above as our service provider.

## 7. Children
The app is not directed at children under 13, and we do not knowingly collect personal information from them.

## 8. Keeping and deleting data
Scan history is kept for the time you choose in Settings (90 days by default), then deleted. Clear history, Forget network, or uninstalling the app removes the data stored by the app. Files you exported are not touched; delete them where you saved them. Firebase keeps crash reports for about 90 days and analytics data according to its retention settings. To ask for deletion of crash or analytics data, write to tecdroiddeveloper@gmail.com with the app instance ID shown in the app's About screen. Deletion page: https://adhavpavan.github.io/app-privacy-policy/wifi-analyzer/delete-data/

## 9. Security
App data is kept in Android's private app storage, which other apps cannot read. Connections to Google services use encryption (HTTPS). Nothing about your network is uploaded by the app.

## 10. Changes
We may update this policy when the app changes. The current version, with its effective date, is always in the app (menu › Privacy policy) and at https://adhavpavan.github.io/app-privacy-policy/wifi-analyzer/.

## 11. Contact
Questions or requests about privacy: tecdroiddeveloper@gmail.com. When you use Contact us, your e-mail app adds the app version, Android version and phone model so we can help.
