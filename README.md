# app-feedback

Bug reports and feature requests for these apps:

| App | Label | Report a bug | Request a feature |
|---|---|---|---|
| Seerr Companion | `app: seerr` | [Bug report](../../issues/new?template=seerr-bug.yml) | [Feature request](../../issues/new?template=seerr-feature.yml) |
| Ephyra | `app: ephyra` | [Bug report](../../issues/new?template=ephyra-bug.yml) | [Feature request](../../issues/new?template=ephyra-feature.yml) |

The quickest way to report a bug is from inside the app: it opens the right form with the app
version and device already filled in.

Everything here is public. Do not post your server's address, an API key, or anyone's name.

## How issues are handled

- Each form adds the app's label, so every issue belongs to exactly one app.
- When an issue becomes work, it gets the `tracked` label and a comment saying so. The fix is
  tracked privately, and this issue is closed with a note when the fix ships.
- `needs-info` means a question is waiting for the reporter.

## Adding an app

1. Add an `app: <id>` label.
2. Add `<id>-bug.yml` and `<id>-feature.yml` under `.github/ISSUE_TEMPLATE/`, copied from an existing
   app. Keep the field ids (`what-happened`, `steps`, `server`, `app-version`, `device`,
   `android-version`), because the apps fill them in from the URL.
3. Add a row to the table above.
