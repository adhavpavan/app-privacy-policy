# App Privacy Policies

Public privacy policies for TechDev Android apps, served with GitHub Pages.

| App | Package | Policy URL |
|---|---|---|
| Focused: Screen Time Control | `com.techdev.focused` | https://adhavpavan.github.io/app-privacy-policy/focused/ · data deletion: https://adhavpavan.github.io/app-privacy-policy/focused/delete-data/ |

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

Focused (`focused-screentime-control` repo):
1. Change the policy in the app repo (bump the effective date) together with the in-app copy
   (`strings_privacy.xml`, `PolicyEffective`), the Accessibility disclosure if its use changed, and the Play docs.
2. Run `scripts/sync_policy.sh` from the app repo: it copies both files here and shows the diff.
3. Here: `git add -A && git commit -m "Update Focused policy: <what changed>" && git push origin main`.
4. Open the URL to check, then update Play Console (Data safety, declarations) to match.

`focused/delete-data/` (account/data deletion page for Play) exists only in this repo.
