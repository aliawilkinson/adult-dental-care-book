# The Adult Teeth Guide: recovery and rebuild

Scope: `product:adult-dental-care-book`. Reviewed 2026-10-06 (America/Los_Angeles; verification 2026-10-07 UTC). Source revision: `a7c862b82520bdf113c00eeeb565878168712b62`. Prepared by Codex from repository evidence; accountable owner review remains pending.

Source authority: [durable context](../context.md), [README](../../README.md), [outline](../../outline.md) and [claims policy](../../claims-policy.md). The dated [backfill report](reports/2026-10-06-backfill-C0-C2.md) scopes verification.

## Failure scenarios

| Failure | First response | Recovery boundary |
| --- | --- | --- |
| Lost workstation | Use an authorized clean machine and recover source at a known SHA | Unpushed edits and independent assets require a separate backup |
| Broken assembled manuscript | Compare chapter history and regenerate manually in outline order | An existing manuscript file alone does not prove equivalence |
| GitHub or Actions unavailable | Continue reviewed local editorial work; queue delivery | Independent backup and account recovery are still needed |
| Published error | Preserve evidence and prepare a reviewed corrected version | Distribution withdrawal is controlled by the chosen channel |

## Complete rebuild procedure

1. Recovery owner obtains GitHub access via the approved account-recovery route. Confirm the repo URL and desired tag/SHA using retained release evidence.
2. Clone into a new empty directory and verify `git rev-parse HEAD`. Inspect `VERSION`, `CHANGELOG.md`, chapter count and the manuscript path.
3. Restore independently held source assets and any uncommitted work from the approved backup into a separate staging directory; compare provenance and hashes before reconciling. This backup and custody are currently unknown.
4. Reconstruct the manuscript from chapters and review documents following [operations](operations.md). Compare with retained release assets using SHA-256, then inspect intended rendering and source references.
5. Recreate the packaging inputs from the exact tagged source and inspect archive membership locally. Resume a release only after the same publication gate as a normal release.
6. Have a second maintainer record start/end time, files recovered, missing work, asset integrity, account-access outcome and author acceptance in a new C5 report.

No end-to-end restore was performed by this backfill. RTO and RPO are **unknown, owner approval required before C3/handoff**. HA and measured app uptime are not applicable because this repository produces documents without a hosted application runtime. GitHub hosting is a dependency, not evidence of independently tested backups.
