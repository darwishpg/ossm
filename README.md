# OSSM Lighthouse — latest version

This repository publishes one file, [`ossm-version.json`](ossm-version.json):
the number of the latest OSSM Lighthouse release. OSSM Lighthouse reads it
from GitHub Pages (`https://darwishpg.github.io/ossm/ossm-version.json`) to
tell its users when a new version is out. It holds nothing else, and nothing
is sent to it.

```json
{
  "version": "1.9.1",
  "critical": false
}
```

- `version`: the latest release, `MAJOR.MINOR.PATCH`.
- `critical`: `true` for a fix every user should install soon; the app says so
  at once.

The releases themselves are in the OSSM Releases folder (P&G sign-in).
Maintainers publish a number only once its package is in that folder, with
`scripts/release/publish_version.py` from the app's repository. To withdraw a
release, the previous number is published again.