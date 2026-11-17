# app-feedback

Bug reports and feature requests for these apps:

| App | Label | Report a bug | Request a feature |
|---|---|---|---|
| Binge | `app: binge` | [Bug report](../../issues/new?template=binge-bug.yml) | [Feature request](../../issues/new?template=binge-feature.yml) |
| Seerr Companion | `app: seerr` | [Bug report](../../issues/new?template=seerr-bug.yml) | [Feature request](../../issues/new?template=seerr-feature.yml) |
| Ephyra | `app: ephyra` | [Bug report](../../issues/new?template=ephyra-bug.yml) | [Feature request](../../issues/new?template=ephyra-feature.yml) |

The quickest way to report a bug is from inside the app: it opens the right form with the app
version and device already filled in.

Everything here is public. Do not post your server's address, an API key, or anyone's name.

## Privacy policies

The apps' privacy policies are published from this repository:

- Seerr Companion: https://scottcooper92.github.io/app-feedback/seerr/privacy/
- Ephyra: https://scottcooper92.github.io/app-feedback/ephyra/privacy/

The published pages are copies of each app's own privacy policy, synced by an automated pull request
from the app's repository when its policy changes; the copy goes live when that PR merges to `main`.
Do not edit a policy here by hand: change it in the app, and the sync brings it over. The front
matter and the "Last updated / Change history" header on each page belong to this site, and the sync
keeps them. The site (index page and policies) lives in `docs/`.

## How issues are handled

- Each form adds the app's label, so every issue belongs to exactly one app.
- When an issue becomes work, it gets the `tracked` label and a comment saying so. The fix is
  tracked privately, and this issue is closed with a note when the fix ships.
- `needs-info` means a question is waiting for the reporter.

## Adding an app

1. Add an `app: <id>` label.
2. Add `<id>-bug.yml` and `<id>-feature.yml` under `.github/ISSUE_TEMPLATE/`, copied from an existing
   app. Keep the field ids the app fills in from the URL (`what-happened`, `steps`, `server`,
   `app-version`, `device`, `android-version`; Binge also sends `platform`, `problem` and `idea`).
3. Add a row to the table above.
