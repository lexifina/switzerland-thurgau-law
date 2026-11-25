<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoring: what is read and what came of it

[Deutsch](README.md)

How global-law monitors every country: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). This page is the same for Thurgau only: every time an official source is read, when, and what came of it (acts added, changed and removed). The machine-readable form is [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` as `Kind: check` commits, and month by month in [checks/](checks/).

**Last check:** 2026-11-25 08:02 UTC, Thurgau: systematic collection (www.rechtsbuch.tg.ch): 115 addresses read; 0 added, 0 changed, 0 removed; no change; 1 not published, 0 of them with no reason.

## Sources

| Source | Folders | How often | Last successful check | Last result | State |
| --- | --- | --- | --- | --- | --- |
| [Thurgau: systematic collection (www.rechtsbuch.tg.ch)](https://www.rechtsbuch.tg.ch/) | `<act>/` | daily | 2026-11-25 08:02 UTC | no change | watched |

## The last 30 days

| Started (UTC) | Source | Read | Added | Changed | Removed | Not published (no reason) | Result | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-25 08:00](checks/2026-11.md#ch-lexwork-thurgau-20261125t080040z) | lexwork-thurgau | 115 | 0 | 0 | 0 | 1 (0) | no change | — |
| [2026-11-24 12:25](checks/2026-11.md#ch-lexwork-thurgau-20261124t122550z) | lexwork-thurgau | 387 | 137 | 0 | 0 | 1 (0) | changes found | [186](https://github.com/lexifina/switzerland-thurgau-law/compare/19e5c6b3f54f...b19f182e788d) |

## Check it yourself

```
python tools/checktrail.py                      # the latest check of every source
python tools/checktrail.py --day 2026-11-23     # every check of a day
python tools/checktrail.py --act <id>           # when an act was seen and published
git log --grep='^Kind: check' --format='%ci %s'  # the checks in the history
```

Only the official publication has legal force; the texts here are copies for reading and searching.
