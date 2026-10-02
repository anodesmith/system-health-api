# Day 7 - System Health Check REST API

> Day 7 of 14 in the **Zero to Production Infrastructure & Security** series.

Lightweight FastAPI service exposing host metrics as JSON for the mobile client built on Day 12.

| | |
|---|---|
| **Day** | 7 of 14 |
| **Status** | Under construction |
| **Verification** | `python -m pytest -q` |
| **Tags** | `python`  `fastapi`  `psutil`  `api`  `monitoring` |

## Focus

- psutil metric collection
- RESTful endpoint design
- Stable JSON response schema
- System-level interaction and error handling

## Status

Implementation lands during the Day 7 build session. Until then this
repository holds the agreed structure only - there is no placeholder code here
pretending to work.

The nightly pipeline appends the real verification result to [STATUS.md](STATUS.md).

## Layout

```
07-system-health-api/
  README.md        this file
  LICENSE          MIT
  STATUS.md        machine-written verification record
  .gitignore       shared from the series root
  .gitattributes   forces LF endings so bash scripts run on Windows
```

## Verify

```bash
python -m pytest -q
```

The nightly job at 22:00 runs this command, records the result and
exit code in STATUS.md, then tags and pushes the repository.

## Licence

MIT. See [LICENSE](LICENSE).