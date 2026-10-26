# App Privacy Policies

Public privacy policies for TechDev Android and iOS apps, served with GitHub Pages.

| App | Package | Policy URL |
|---|---|---|
| Focused: Screen Time Control | `com.techdev.focused` | https://adhavpavan.github.io/app-privacy-policy/focused/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/focused/delete-data/ |
| Focused: Screen Time Control (iOS) | `com.techdev.focused` | https://adhavpavan.github.io/app-privacy-policy/focused-ios/ (no data collected, so no deletion page) |
| Corelyze: CPU & Device Info | `com.techdev.corelyze` | https://adhavpavan.github.io/app-privacy-policy/corelyze/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/corelyze/delete-data/ |
| Chargewise: Battery Health | `com.techdev.chargewise` | https://adhavpavan.github.io/app-privacy-policy/chargewise/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/chargewise/delete-data/ |
| Measurely: Sound, Level, Lux | `com.techdev.measurely` | https://adhavpavan.github.io/app-privacy-policy/measurely/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/measurely/delete-data/ |
| Northwise: Digital Compass | `com.techdev.northwise` | https://adhavpavan.github.io/app-privacy-policy/northwise/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/northwise/delete-data/ |
| Decibly: Sound Meter & dB | `com.techdev.decibly` | https://adhavpavan.github.io/app-privacy-policy/decibly/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/decibly/delete-data/ |

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
| Focused iOS | `focused-ios/docs/policy/privacy-policy.md`, `privacy-policy.html` | `focused-ios/privacy-policy.md`, `focused-ios/index.html` |
| Corelyze | `docs/playstore/policy/privacy-policy.md` (HTML rendered by `scripts/policy_md2html.py`) | `corelyze/privacy-policy.md`, `corelyze/index.html` |
| Chargewise | `docs/playstore/policy/privacy-policy.md`, `privacy-policy.html` | `chargewise/privacy-policy.md`, `chargewise/index.html` |
| Measurely | `docs/playstore/policy/privacy-policy.md` (HTML rendered by `scripts/policy_md2html.py`) | `measurely/privacy-policy.md`, `measurely/index.html` |
| Northwise | `docs/playstore/policy/privacy-policy.md` (HTML rendered by `scripts/policy_md2html.py`) | `northwise/privacy-policy.md`, `northwise/index.html` |
| Decibly | `docs/playstore/policy/privacy-policy.md` (HTML rendered by `scripts/policy_md2html.py`) | `decibly/privacy-policy.md`, `decibly/index.html` |

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
