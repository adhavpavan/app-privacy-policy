# App Privacy Policies

Public privacy policies for TechDev Android and iOS apps, served with GitHub Pages.

| App | Package | Policy URL |
|---|---|---|
| Focused: Screen Time Control | `com.techdev.focused` | https://adhavpavan.github.io/app-privacy-policy/focused/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/focused/delete-data/ |
| Focused: Control Your Time (iOS) | `com.techdev.focused` | https://adhavpavan.github.io/app-privacy-policy/focused-ios/ (no data collected, so no deletion page) · support: https://adhavpavan.github.io/app-privacy-policy/focused-ios/support/ |
| Corelyze: CPU & Device Info | `com.techdev.corelyze` | https://adhavpavan.github.io/app-privacy-policy/corelyze/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/corelyze/delete-data/ |
| Chargewise: Battery Health | `com.techdev.chargewise` | https://adhavpavan.github.io/app-privacy-policy/chargewise/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/chargewise/delete-data/ |
| Measurely: Sound, Level, Lux | `com.techdev.measurely` | https://adhavpavan.github.io/app-privacy-policy/measurely/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/measurely/delete-data/ |
| Northwise: Digital Compass | `com.techdev.northwise` | https://adhavpavan.github.io/app-privacy-policy/northwise/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/northwise/delete-data/ |
| Decibly: Sound Meter & dB | `com.techdev.decibly` | https://adhavpavan.github.io/app-privacy-policy/decibly/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/decibly/delete-data/ |
| Data Manager and App Usage | `com.techdev.internetspeedmeter` | https://adhavpavan.github.io/app-privacy-policy/data-manager/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/data-manager/delete-data/ |
| WiFi Analyzer & Who's on WiFi | `com.techdev.wifianalyzer` | https://adhavpavan.github.io/app-privacy-policy/wifi-analyzer/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/wifi-analyzer/delete-data/ |
| Voice Recorder | `com.techdev.voicerecorder` | https://adhavpavan.github.io/app-privacy-policy/voice-recorder/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/voice-recorder/delete-data/ |
| Compress Image | `com.techdev.compressimage` | https://adhavpavan.github.io/app-privacy-policy/compress-image/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/compress-image/delete-data/ |
| Image Converter | `com.techdev.imageconverter` | https://adhavpavan.github.io/app-privacy-policy/image-converter/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/image-converter/delete-data/ |
| QR Code Scanner & Generator | `com.techdev.qrscanner` | https://adhavpavan.github.io/app-privacy-policy/qr-scanner/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/qr-scanner/delete-data/ |
| Spokenote: AI Voice Recorder (iOS) | `com.techdev.spokenote` | https://adhavpavan.github.io/app-privacy-policy/spokenote/ (no data collected) · support: https://adhavpavan.github.io/app-privacy-policy/spokenote/support/ |
| WiFi Analyzer & Who's on WiFi (iOS, iPadOS, macOS) | `com.techdev.wifianalyzer` | https://adhavpavan.github.io/app-privacy-policy/wifi-analyzer-ios/ (no data collected) · support: https://adhavpavan.github.io/app-privacy-policy/wifi-analyzer-ios/support/ |
| ScanIt: QR & Barcode Reader (iOS, formerly QR Buddy) | `com.techdev.qrbuddy` | https://adhavpavan.github.io/app-privacy-policy/qrbuddy/ (no data collected) · support: https://adhavpavan.github.io/app-privacy-policy/qrbuddy/support/ |
| Remote-IO: TV Remote Control (iOS) | `com.techdev.remotio` | https://adhavpavan.github.io/app-privacy-policy/remotio/ (no data collected) · support: https://adhavpavan.github.io/app-privacy-policy/remotio/support/ |
| Chiplens: Device Info & Specs (iOS, iPadOS, macOS) | `com.techdev.chiplens` | https://adhavpavan.github.io/app-privacy-policy/chiplens/ (no data collected) · support: https://adhavpavan.github.io/app-privacy-policy/chiplens/support/ |
| Long Screenshot & Stitch (iOS, iPadOS; project Fullscroll) | `com.techdev.fullscroll` | https://adhavpavan.github.io/app-privacy-policy/fullscroll/ (no data collected) · support: https://adhavpavan.github.io/app-privacy-policy/fullscroll/support/ |
| WidgetWell: Aesthetic Widgets (iOS, iPadOS, visionOS, watchOS) | `com.techdev.widgetwell` | https://adhavpavan.github.io/app-privacy-policy/widgetwell/ (no data collected) · support: https://adhavpavan.github.io/app-privacy-policy/widgetwell/support/ |

## Hosting

GitHub → Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.

## Adding an app

Create `<app>/index.html` (and the Markdown source next to it), add a link in `index.html` and a row above.
One folder per app; each gets its own URL `https://adhavpavan.github.io/app-privacy-policy/<app>/`.

## Updating a policy

Every push to `main` republishes the site (GitHub Pages, about a minute). Never edit a policy only here:
the source of truth is the app repo.

| App | Source in app repo | Copied to |
|---|---|---|
| Focused | `docs/playstore/policy/privacy-policy.md`, `privacy-policy.html` | `focused/privacy-policy.md`, `focused/index.html` |
| Focused iOS | `focused-ios/docs/policy/privacy-policy.md`, `privacy-policy.html`, `support.html` | `focused-ios/privacy-policy.md`, `focused-ios/index.html`, `focused-ios/support/index.html` |
| Fullscroll | `screenshot-stitch-ios/docs/policy/privacy-policy.md`, `privacy-policy.html`, `support.html` (copied by `scripts/sync_policy.sh`) | `fullscroll/privacy-policy.md`, `fullscroll/index.html`, `fullscroll/support/index.html` |
| WidgetWell | `all-in-one-widgets-ios/docs/policy/privacy-policy.md`, `privacy-policy.html`, `support.html` (copied by `scripts/sync_policy.sh`) | `widgetwell/privacy-policy.md`, `widgetwell/index.html`, `widgetwell/support/index.html` |
| Corelyze | `docs/playstore/policy/privacy-policy.md` (HTML rendered by `scripts/policy_md2html.py`) | `corelyze/privacy-policy.md`, `corelyze/index.html` |
| Chargewise | `docs/playstore/policy/privacy-policy.md`, `privacy-policy.html` | `chargewise/privacy-policy.md`, `chargewise/index.html` |
| Measurely | `docs/playstore/policy/privacy-policy.md` (HTML rendered by `scripts/policy_md2html.py`) | `measurely/privacy-policy.md`, `measurely/index.html` |
| Northwise | `docs/playstore/policy/privacy-policy.md` (HTML rendered by `scripts/policy_md2html.py`) | `northwise/privacy-policy.md`, `northwise/index.html` |
| Decibly | `docs/playstore/policy/privacy-policy.md` (HTML rendered by `scripts/policy_md2html.py`) | `decibly/privacy-policy.md`, `decibly/index.html` |
| Data Manager | `docs/playstore/policy/privacy-policy.md` (HTML rendered by `scripts/policy_md2html.py`) | `data-manager/privacy-policy.md`, `data-manager/index.html` |
| WiFi Analyzer | In-app copy in `wifi-analyser-whos-on-wifi`: `strings_privacy.xml`, `strings_privacy_wifi.xml` (effective 1 November 2026). `docs/playstore/policy/` is not in that repo yet | `wifi-analyzer/privacy-policy.md`, `wifi-analyzer/index.html` |
| Voice Recorder | In-app copy in `voice-recorder`: `strings_privacy.xml`, `strings_app_voice.xml` (effective 1 November 2026) | `voice-recorder/privacy-policy.md`, `voice-recorder/index.html` |
| Compress Image | In-app copy in `compress-image-pdf`: `strings_privacy.xml` (effective 1 November 2026) | `compress-image/privacy-policy.md`, `compress-image/index.html` |
| Image Converter | In-app copy in `image-pdf-converter`: `strings_privacy.xml` (effective 1 November 2026) | `image-converter/privacy-policy.md`, `image-converter/index.html` |
| QR Scanner | `qr-code-scannar/docs/playstore/policy/privacy-policy.md`, `privacy-policy.html` | `qr-scanner/privacy-policy.md`, `qr-scanner/index.html` |
| Spokenote (iOS) | `new-apps/voice-notes-ai/docs/policy/privacy-policy.md`, `privacy-policy.html`, `support.html` | `spokenote/privacy-policy.md`, `spokenote/index.html`, `spokenote/support/index.html` |
| ScanIt (iOS) | `new-apps/qr-barcode-kit/docs/policy/privacy-policy.md`, `privacy-policy.html`, `support.html` | `qrbuddy/privacy-policy.md`, `qrbuddy/index.html`, `qrbuddy/support/index.html` |
| Remotio (iOS) | `new-apps/universal-tv-remote/docs/policy/privacy-policy.md`, `privacy-policy.html`, `support.html` | `remotio/privacy-policy.md`, `remotio/index.html`, `remotio/support/index.html` |
| Chiplens (iOS) | `new-apps/research/device-info-ios/docs/policy/privacy-policy.md`, `privacy-policy.html`, `support.html` | `chiplens/privacy-policy.md`, `chiplens/index.html`, `chiplens/support/index.html` |

Focused (`focused-screentime-control` repo):
1. Change the policy in the app repo (bump the effective date) together with the in-app copy
   (`strings_privacy.xml`, `PolicyEffective`), the Accessibility disclosure if its use changed, and the Play docs.
2. Run `scripts/sync_policy.sh` from the app repo: it copies both files here and shows the diff.
3. Here: `git add -A && git commit -m "Update Focused policy: <what changed>" && git push origin main`.
4. Open the URL to check, then update Play Console (Data safety, declarations) to match.

`focused/delete-data/`, `corelyze/delete-data/`, `chargewise/delete-data/`, `measurely/delete-data/`, `northwise/delete-data/` and `decibly/delete-data/` (data deletion pages for Play) exist only in this repo.

Corelyze (`DeviceInfo/android-device-info` repo): same steps; `scripts/sync_policy.sh` re-renders the HTML from the Markdown and copies both here.

Chargewise (`android-battery-health` repo): same steps; `scripts/sync_policy.sh` copies both files here.

Measurely (`sensor-toolbox` repo): same steps; render the HTML with `scripts/policy_md2html.py` first, then
`scripts/sync_policy.sh` copies both files here.

Northwise (`new-apps/digital-compass` repo): same steps; render the HTML with
`python3 -I scripts/policy_md2html.py docs/playstore/policy/privacy-policy.md docs/playstore/policy/privacy-policy.html docs/playstore/policy/privacy-policy.html`
first, then `scripts/sync_policy.sh` copies both files here.

Decibly (`new-apps/sound-meter` repo): same steps; render the HTML with
`python3 -I scripts/policy_md2html.py docs/playstore/policy/privacy-policy.md docs/playstore/policy/privacy-policy.html docs/playstore/policy/privacy-policy.html`
first, then `scripts/sync_policy.sh` copies both files here.

Data Manager (`Pavan_ISM/InternetSpeedMeter` repo): same steps; `scripts/sync_policy.sh` re-renders the HTML from the
Markdown and copies both here. The in-app copy is the `privacy_*` strings in `strings_settings.xml` (all locales).
`data-manager/delete-data/` exists only in this repo.

`wifi-analyzer/delete-data/`, `voice-recorder/delete-data/`, `compress-image/delete-data/`, `image-converter/delete-data/` and `qr-scanner/delete-data/` (data deletion pages for Play) exist only in this repo. The pages were first published on 8 November 2026 from each app's in-app policy. QR Scanner's page is a copy of `qr-code-scannar/docs/playstore/policy/`.
