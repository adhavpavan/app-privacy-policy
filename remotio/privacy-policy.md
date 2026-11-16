# Privacy Policy — Remotio for iPhone and iPad

Effective date: 2026-11-16

**In short:** Remotio collects no data. No account, no servers of ours, no ads, no analytics, no tracking. The app
talks only to the TV on your home network and, if you allow it, to Apple Home (HomeKit) on your own devices.

This policy explains how Remotio ("the app", "we"), bundle ID `com.techdev.remotio`, handles information.
Published at https://adhavpavan.github.io/app-privacy-policy/remotio/ (support: `/remotio/support/`).

## 1. What the app uses, and where it stays

| Information | Why | Where it stays |
|---|---|---|
| Your TV list: name you gave it, brand/platform, model, IP address on your network, network (MAC) address if the TV reports it | To find and reconnect to your TV; the MAC address is for waking the TV over the network where supported | On your device, in the app's shared storage (also read by the app's own widgets and controls) |
| Pairing keys your TV gives the app (Samsung token, LG key, Fire TV token) and the app's own security certificate for Google TV / Android TV | So you don't have to approve or type a code every time | In the iOS Keychain on this device only; not synced to iCloud |
| Remote buttons you press, and text you type in the keyboard screen | To control your TV | Sent directly to your TV over your Wi-Fi. Not stored, not sent anywhere else |
| Settings (appearance, accent, haptics, remote options, chosen home and TV room, demo home on/off) | To remember your choices | On your device |
| Apple Home data, only if you allow HomeKit access: names of your homes, rooms, accessories and scenes, and their current state (on/off, temperature, mode, brightness…) | To show and control your air conditioners, lights and scenes in the Home tab | Read from Apple Home on your device. Commands go to your accessories through Apple Home. Never sent to us |
| A short copy of your ACs' and scenes' names and last-known state | So the app's own widgets, Control Center controls and Siri can show and list them | On your device, in the app's shared storage. Not sent anywhere |

We do not collect your name, e-mail address, contacts, location, photos, microphone, or any identifier.

## 2. Local network

To find your TV and send buttons to it, Remotio needs iOS **Local Network** access. With it, the app:
- looks for TVs with Bonjour (the same discovery AirPlay uses) and by briefly checking addresses on your own Wi-Fi
  network for the ports smart TVs use (for example Roku, Samsung, LG, Google TV and Fire TV remote ports);
- reads basic, public information TVs share on the network (name, model, network address) to show them in a list;
- sends remote commands and typed text to the TV you chose.

None of this traffic leaves your home network. You can turn Local Network off any time in Settings › Remotio; the
demo TV still works.

## 3. Apple Home (HomeKit)

The **Home** tab shows accessories and scenes from Apple Home. The app asks for HomeKit access only when you open
that tab and tap Continue. With it, the app reads your homes, rooms, accessories and scenes, changes accessories
when you tap them (for example the AC temperature), runs scenes, and creates a "Movie mode" scene **only after you
confirm** the list of what it does. HomeKit is Apple's framework: your home data is stored and synced by Apple Home
on your devices (and iCloud, if you use it). Remotio has no server; nothing about your home is sent to us or to
anyone else. iPhone has no infrared; the app controls only accessories that are in Apple Home. If you don't allow
access, the TV remote works as before and the Home tab offers a demo home with made-up accessories. You can change
the permission any time in Settings › Remotio.

## 4. Other permissions

- **Face ID / Touch ID** (optional App lock): iOS checks it; the app only learns whether it succeeded.
- **Live Activities** (optional Lock Screen remote): shown only when you turn it on from the remote screen.

The app does not ask for notifications, microphone, camera, photos, location or contacts.

## 5. Third-party services

None. The app contains no third-party analytics, advertising, crash-reporting or tracking software, and no ad SDK.
If you share analytics with developers in iOS settings, Apple may send us anonymous crash reports. Once a day the
app asks Apple's App Store whether a newer version exists; that request contains only the app's ID and your store
country. TV brand names are trademarks of their owners; Remotio is not affiliated with any TV maker.

## 6. Sharing, selling, children

We do not sell, rent or share any information. The app collects no personal information from anyone, including
children.

## 7. Keeping and deleting data

Everything stays on your device and in your own device backups (Keychain items are device-only). To remove it:
TVs › swipe a TV › Forget (removes the TV and its pairing keys), Settings › Forget all pairings, or delete the app.
Your Apple Home data is managed in Apple's Home app; deleting Remotio does not change it (a Movie mode scene you
created stays in the Home app until you delete it there).

## 8. Changes

We update this page when the app changes; the effective date is at the top.

## 9. Contact

tecdroiddeveloper@gmail.com
