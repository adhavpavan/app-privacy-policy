# Privacy Policy — Remote-IO for iPhone, iPad and Apple Watch

Effective date: 2026-11-21

**In short:** Remote-IO collects no data. No account, no servers of ours, no ads, no analytics, no tracking. The app
talks only to your TV and the smart-home devices you add on your home network and, if you allow it, to Apple Home
(HomeKit) on your own devices. If you keep iCloud sync on, your TV list and pairings are kept in **your own** iCloud
by Apple, where we can't see them.

This policy explains how Remote-IO ("the app", "we"), bundle ID `com.techdev.remotio`, handles information.
Published at https://adhavpavan.github.io/app-privacy-policy/remotio/ (support: `/remotio/support/`).

## 1. What the app uses, and where it stays

| Information | Why | Where it stays |
|---|---|---|
| Your TV list: name you gave it, brand/platform, model, IP address on your network, network (MAC) address if the TV reports it | To find and reconnect to your TV; the MAC address is for waking the TV over the network where supported | On your device, in the app's shared storage (also read by the app's own widgets and controls). With iCloud sync on (section 4), also in your own iCloud |
| Pairing keys your TV gives the app (Samsung token, LG key, Fire TV token) and the app's own security certificate for Google TV / Android TV | So you don't have to approve or type a code every time | In the iOS Keychain. With iCloud sync on (default), in your iCloud Keychain (end-to-end encrypted by Apple) so your other iPhone and iPad don't need to pair again; with it off, on this device only |
| Remote buttons you press, and text you type in the keyboard screen | To control your TV | Sent directly to your TV over your Wi-Fi. Not stored, not sent anywhere else |
| Settings (appearance, accent, haptics, remote options, chosen home and TV room, demo home on/off), and the apps and shortcuts you pin for each TV | To remember your choices | On your device. With iCloud sync on, appearance, accent, tabs, haptics and remote options also in your own iCloud |
| Room scenes you make ("Movie night": name, icon, steps naming a TV, input, app, volume, Home device or scene) | To run your TV and Home devices together in one tap | On your device, in the app's shared storage. With iCloud sync on (section 4), also in your own iCloud |
| Apple Home data, only if you allow HomeKit access: names of your homes, rooms, accessories and scenes, and their current state (on/off, temperature, mode, brightness…) | To show and control your air conditioners, lights and scenes in the Home tab | Read from Apple Home on your device. Commands go to your accessories through Apple Home. Never sent to us |
| Wi-Fi smart-home devices you add (Philips Hue bridge, Shelly, Nanoleaf, WLED, Elgato, WiZ, Yeelight, Govee, LIFX): name, type, room, IP address on your network, and the pairing key some of them give the app | To show and control them in the Home tab without Apple Home or any account | Device list on your device, in the app's shared storage; pairing keys in the iOS Keychain on this device only, unless you turn on "Also sync Home device keys" (then in your iCloud Keychain). Commands go directly to the device over your Wi-Fi |
| Your own Home Assistant server, if you connect it: its address on your network and the long-lived access token you paste | To show and control the devices and scenes your Home Assistant manages | Address in the app's shared storage on your device; token in the iOS Keychain on this device only (or your iCloud Keychain if you turn on "Also sync Home device keys"). The token is sent only to your Home Assistant on your home network, never to us or anyone else. Delete it any time in Home Assistant or by removing it in Remote-IO |
| On Apple Watch: your TV names, which TV is current, and your accent colour; the buttons you press on the watch | So the watch remote can show your TVs by name and send buttons | Passed between your iPhone and your paired Apple Watch by Apple's WatchConnectivity (direct, not through any server of ours). The watch can't reach the TV itself: each press goes to Remote-IO on your iPhone, which sends it to the TV over your Wi-Fi. Nothing is stored on the watch beyond what iOS keeps for that connection |
| A short copy of your ACs' and scenes' names and last-known state | So the app's own widgets, Control Center controls and Siri can show and list them | On your device, in the app's shared storage. Not sent anywhere |

We do not collect your name, e-mail address, contacts, location, photos, voice recordings, or any identifier.

## 2. Local network

To find your TV and send buttons to it, Remote-IO needs iOS **Local Network** access. With it, the app:
- looks for TVs with Bonjour (the same discovery AirPlay uses) and by briefly checking addresses on your own Wi-Fi
  network for the ports smart TVs use (for example Roku, Samsung, LG, Google TV and Fire TV remote ports);
- reads basic, public information TVs share on the network (name, model, network address) to show them in a list;
- sends remote commands and typed text to the TV you chose;
- finds, pairs with and controls the Wi-Fi smart-home devices you add in the Home tab (Bonjour, or the IP address
  you type).

None of this traffic leaves your home network. You can turn Local Network off any time in Settings › Remote-IO; the
demo TV still works.

## 3. Apple Home (HomeKit)

The **Home** tab shows accessories and scenes from Apple Home. The app asks for HomeKit access only when you open
that tab and tap Continue. With it, the app reads your homes, rooms, accessories and scenes, changes accessories
when you tap them (for example the AC temperature), runs scenes, and creates a "Movie mode" scene **only after you
confirm** the list of what it does. HomeKit is Apple's framework: your home data is stored and synced by Apple Home
on your devices (and iCloud, if you use it). Remote-IO has no server; nothing about your home is sent to us or to
anyone else. iPhone has no infrared. Without Apple Home access, the TV remote and the Wi-Fi devices you add still work,
and you can try a demo home with made-up accessories. You can change
the permission any time in Settings › Remote-IO.

## 4. iCloud sync

Settings › iCloud › **Sync TVs and pairings with iCloud** (on by default) keeps your TV list (names, brand/platform,
model, network address, MAC address if known), your room scenes (name, icon and steps, which name a TV or Home
device by its id) and a few settings (appearance, accent, tabs, haptics, remote options) in your own iCloud
key-value storage, and the TV pairing keys in your **iCloud Keychain**, which Apple encrypts end to
end. Your Apple Account is the only account: Remote-IO has no server, and **the developer has no access** to any of it.
Pairing keys of Wi-Fi Home devices (Hue, Nanoleaf, Home Assistant) sync only if you also turn on **Also sync Home
device keys** (off by default).
Turn sync off any time: this device keeps its own copy and stops syncing, and your other devices keep the copies
already in your iCloud. To remove pairing keys from iCloud Keychain too, use Settings › Forget all pairings while sync is
on. If you're not signed in to iCloud, nothing syncs and the app works the same.

## 5. Other permissions

- **Face ID / Touch ID** (optional App lock): iOS checks it; the app only learns whether it succeeded.
- **Live Activities** (optional Lock Screen remote): shown only when you turn it on from the remote screen.
- **Apple Watch** (optional): the watch app asks for no permissions; it works through Remote-IO on your iPhone.
- **Microphone and Speech Recognition** (optional voice search): asked only when you first tap the microphone.
  Your speech is turned into text **on your device** by Apple's on-device speech recognition; the text goes only to
  your TV as a search. No audio is stored or sent to us or anyone else.
- **Share to Remote-IO** (optional share extension): when you share a link to Remote-IO from another app, it sends
  that link **only to your TV on your home network** so the TV can open it. Nothing is stored or sent anywhere else.

The app does not ask for notifications, camera, photos, location or contacts.

## 6. Third-party services

None. The app contains no third-party analytics, advertising, crash-reporting or tracking software, and no ad SDK.
If you share analytics with developers in iOS settings, Apple may send us anonymous crash reports. Once a day the
app asks Apple's App Store whether a newer version exists; that request contains only the app's ID and your store
country. TV brand names are trademarks of their owners; Remote-IO is not affiliated with any TV maker.

## 7. Sharing, selling, children

We do not sell, rent or share any information. The app collects no personal information from anyone, including
children.

## 8. Keeping and deleting data

Everything stays on your device, in your own device backups and, with iCloud sync on, in your own iCloud. To remove
it: TVs › swipe a TV › Forget (removes the TV and its pairing keys, also from your other devices when sync is on),
Settings › Forget all pairings, Settings › iCloud (turn sync off), or delete the app.
Your Apple Home data is managed in Apple's Home app; deleting Remote-IO does not change it (a Movie mode scene you
created stays in the Home app until you delete it there).

## 9. Changes

We update this page when the app changes; the effective date is at the top.

## 10. Contact

tecdroiddeveloper@gmail.com
