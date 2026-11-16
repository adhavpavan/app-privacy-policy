# Privacy Policy — Fairmote for iPhone and iPad

Effective date: 2026-11-16

**In short:** Fairmote collects no data. No account, no servers of ours, no ads, no analytics, no tracking. The app
talks only to the TV on your home network.

This policy explains how Fairmote ("the app", "we"), bundle ID `com.techdev.fairmote`, handles information.
Published at https://adhavpavan.github.io/app-privacy-policy/fairmote/ (support: `/fairmote/support/`).

## 1. What the app uses, and where it stays

| Information | Why | Where it stays |
|---|---|---|
| Your TV list: name you gave it, brand/platform, model, IP address on your network, network (MAC) address if the TV reports it | To find and reconnect to your TV; the MAC address is for waking the TV over the network where supported | On your device, in the app's shared storage (also read by the app's own widgets and controls) |
| Pairing keys your TV gives the app (Samsung token, LG key, Fire TV token) and the app's own security certificate for Google TV / Android TV | So you don't have to approve or type a code every time | In the iOS Keychain on this device only; not synced to iCloud |
| Remote buttons you press, and text you type in the keyboard screen | To control your TV | Sent directly to your TV over your Wi-Fi. Not stored, not sent anywhere else |
| Settings (appearance, accent, haptics, remote options) | To remember your choices | On your device |

We do not collect your name, e-mail address, contacts, location, photos, microphone, or any identifier.

## 2. Local network

To find your TV and send buttons to it, Fairmote needs iOS **Local Network** access. With it, the app:
- looks for TVs with Bonjour (the same discovery AirPlay uses) and by briefly checking addresses on your own Wi-Fi
  network for the ports smart TVs use (for example Roku, Samsung, LG, Google TV and Fire TV remote ports);
- reads basic, public information TVs share on the network (name, model, network address) to show them in a list;
- sends remote commands and typed text to the TV you chose.

None of this traffic leaves your home network. You can turn Local Network off any time in Settings › Fairmote; the
demo TV still works.

## 3. Other permissions

- **Face ID / Touch ID** (optional App lock): iOS checks it; the app only learns whether it succeeded.
- **Live Activities** (optional Lock Screen remote): shown only when you turn it on from the remote screen.

The app does not ask for notifications, microphone, camera, photos, location, contacts or HomeKit.

## 4. Third-party services

None. The app contains no third-party analytics, advertising, crash-reporting or tracking software, and no ad SDK.
If you share analytics with developers in iOS settings, Apple may send us anonymous crash reports. Once a day the
app asks Apple's App Store whether a newer version exists; that request contains only the app's ID and your store
country. TV brand names are trademarks of their owners; Fairmote is not affiliated with any TV maker.

## 5. Sharing, selling, children

We do not sell, rent or share any information. The app collects no personal information from anyone, including
children.

## 6. Keeping and deleting data

Everything stays on your device and in your own device backups (Keychain items are device-only). To remove it:
TVs › swipe a TV › Forget (removes the TV and its pairing keys), Settings › Forget all pairings, or delete the app.

## 7. Changes

We update this page when the app changes; the effective date is at the top.

## 8. Contact

tecdroiddeveloper@gmail.com
