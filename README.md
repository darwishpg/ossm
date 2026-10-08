# OSSM latest version

```json
{
  "version": "1.9.1",
  "critical": false
}
```

- `version`: the latest release, `MAJOR.MINOR.PATCH`.
- `critical`: `true` for a fix every user should install soon; the app says so
  at once.

Maintainers publish a number only once its package is in that folder, with
`scripts/release/publish_version.py` from the app's repository. To withdraw a
release, the previous number is published again.
