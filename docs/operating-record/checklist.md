# The Adult Teeth Guide: checkpoint checklist

Scope: `product:adult-dental-care-book`. Reviewed 2026-10-06 (America/Los_Angeles; verification 2026-10-07 UTC). Source revision: `a7c862b82520bdf113c00eeeb565878168712b62`. Prepared by Codex from repository evidence; accountable owner review remains pending.

Follow the adopted [Product Factory standard](../product-operating-record-standard.md). Start here at each milestone; update affected diagrams/runbooks in the same PR as the source change and copy the [report template](reports/TEMPLATE.md) to a dated checkpoint report. This pack is a substantive backfill, not retroactive approval of a release.

## Source authority and accountability

Durable business/source context: [durable context](../context.md), [README](../../README.md), [outline](../../outline.md) and [claims policy](../../claims-policy.md). Canonical identities are listed in [architecture](architecture.md). Product/Workspace contact is Alia; named support, recovery and reviewer assignments require owner confirmation. Roles below identify who must close each gap, not an invented staffing commitment. Criticality: Editorial continuity and source preservation are the current critical journeys. Loss interrupts writing and evidence review. A published error has a different impact from an unavailable draft. No reader service availability target is established.

## C0 through C5

| Checkpoint and trigger | Existing deliverable / evidence | Exit status |
| --- | --- | --- |
| C0: intake or adoption | Purpose, audience, ownership references, criticality and scope in context and architecture | Open: owner/recovery assignments and relevant identity gaps below |
| C1: before architecture/tooling change | System context, source/tooling and delivery views in architecture; failure behavior in recovery | Documented baseline; targets and unresolved design choices remain open |
| C2: every implementation/editorial milestone | Concrete setup, verification, release/correction and recovery procedures; dated backfill report | Mechanical checks scoped in report; broader content and recovery evidence remain open |
| C3: before public release, paid pilot or production promotion | Candidate SHA/artifacts, applicable reviews, rights/access, rollback/correction and recovery rehearsal | Hold until applicable gaps and actual owner signoff are recorded |
| C4: after release and agreed observation window | Actual tag/edition/artifact hash, destination/environment, smoke/readability result, observations and MetadataDB acknowledgement | Unknown for prior distribution; this backfill performs no release |
| C5: change, handoff, recovery drill, dormancy or retirement | Updated record, custody/obligations, tested restoration and receiving-maintainer acceptance | Open: independent recovery and handoff not tested |

Completed deliverables, not completed checkpoint approvals:

- [x] [Architecture](architecture.md) describes real paths and distinguishes intended, implemented and observed claims.
- [x] [Operations](operations.md) provides repository-specific setup, verification, delivery, correction and maintenance steps.
- [x] [Recovery](recovery.md) documents failures, rebuild order, missing custody/targets and acceptance criteria.
- [x] [Dated report](reports/2026-10-06-backfill-C0-C2.md) records exact source and actual limited checks.
- [ ] Confirm role assignments and criticality/target decisions.
- [ ] Rehearse independent recovery and resolve applicable release gaps.
- [ ] Obtain scoped human Signoff and, after real release, preserve receipt/observation evidence.

## Open gates

Every item is **unknown or incomplete**, unless the linked report later supersedes it. The owner sets calendar due dates at milestone planning; none are invented here. Until then, the named gate is the deadline and stays open.

| Gap | Responsible role | Required by gate | Required evidence/action |
| --- | --- | --- | --- |
| 1 | Product / Alia | C0 and C3 | Confirm backup custodian, delegated recovery contact and publication support route. |
| 2 | Editorial owner / qualified reviewer | C3 | Resolve applicable claim/source and author-decision reports for the exact release candidate; this backfill performs no medical review. |
| 3 | Release owner | C3 | Reconcile chapter sources with the assembled manuscript and approve all files included in the public source archive. |
| 4 | Recovery owner / Alia | C3 and C5 | Approve recovery time/data-loss targets, independent backup custody and an off-device restore drill. |
| 5 | Release owner | C4 | Record actual immutable release assets, distribution target and MetadataDB acknowledgement; workflow source alone proves none of these. |

## Maintenance rule

At a source/toolchain/dependency, ownership, rights, data or distribution change, update only the affected record and add a new report. Keep previous reports intact. Document `not-applicable` with a reason, separate `documented` from `verified`, and keep credentials/private source content out of operational evidence. Link this pack into MetadataDB through its reviewed ingestion path; catalog acknowledgement remains unknown until returned. Recovery documentation stays usable locally even when the catalog is unavailable.
