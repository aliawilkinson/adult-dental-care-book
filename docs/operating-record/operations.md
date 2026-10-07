# The Adult Teeth Guide: operating procedures

Scope: `product:adult-dental-care-book`. Reviewed 2026-10-06 (America/Los_Angeles; verification 2026-10-07 UTC). Source revision: `a7c862b82520bdf113c00eeeb565878168712b62`. Prepared by Codex from repository evidence; accountable owner review remains pending.

Source authority: [durable context](../context.md), [README](../../README.md), [outline](../../outline.md) and [claims policy](../../claims-policy.md). The dated [backfill report](reports/2026-10-06-backfill-C0-C2.md) scopes verification.

## Start or hand off editorial work

Clone `https://github.com/aliawilkinson/adult-dental-care-book.git` into an authorized location, record the branch and SHA, then read [AGENTS.md](../../AGENTS.md) and its named editorial documents before manuscript changes. Work through a branch and PR. Read [reviews/progress.md](../../reviews/progress.md) to select the next chapter and retain existing author decisions. A Markdown editor and Git are enough for the current manual authoring path; no application install, environment file or database migration is required.

## Assemble and verify

1. Select the exact candidate SHA and inspect every chapter against [outline.md](../../outline.md).
2. Follow the whole-book review in AGENTS.md to assemble `book/full-manuscript.md` in approved order, with one title page. There is no automated assembly command to run or claim as tested.
3. Review applicable existing fact-check, source-needs, continuity and author-decision files under `reviews/`; record reviewer and resolved/open decisions. Keep substantive review separate from file-existence checks.
4. Check headings, cross-references, citations, cheat-sheet consistency and rendering in the intended export format. Final PDF/e-book/print toolchain and accessibility acceptance are unknown.
5. Inspect the exact source archive allowlist in `release.yml`. It includes `docs`, `research`, `reviews` and `sources`; internal-only material cannot be treated as excluded from a public archive.

## Release and correction

The existing workflow uses Conventional Commit history to open a Release Please PR. Its merge creates the version/tag; packaging checks out `needs.release.outputs.sha`, copies the manuscript and creates the source tar archive. The shared publish workflow attaches release assets. Record workflow run URL, tag, SHA, asset names/hashes and the actual destination only after success. A PR merge or prepared package is not publication evidence.

For an error discovered before release, revise the chapter and assembled manuscript together on a branch. For an error in an already published artifact, retain the old tag/evidence, prepare a corrected version and an erratum, and let the release owner decide channel correction or withdrawal. Channel access and retailer rollback steps are unknown until a distribution target is chosen. Never rewrite an immutable release to hide a correction.

## Data, access and maintenance

The repo holds authored content and source/review notes, not customer dental records. GitHub owner access is required for merge/release; delegated recovery and MFA recovery locators are unknown and belong in an owner-approved access store, never in this pack. Ownership is `person:alia` in MetadataDB; third-party quotations, illustrations and source permissions require editorial review before their inclusion.

At each chapter milestone, update source needs and the C2 report. Before release, review claim freshness, permissions, artifact contents and export accessibility. On GitHub/shared-workflow changes, recheck permissions, artifact retention and the packaging boundary. Costs may include Actions, editing, layout, art and distribution; plan, balances, amounts and renewals were not inspected. The owner records obligations and renewal reminders in MetadataDB when established. No scheduled review date or paid plan is invented here.

For retirement, retain approved source, release hashes, corrections and permission records in an independently recoverable store, document where readers can obtain the final version, and transfer account custody before removing access.

## Publishing and commercial preparation

Follow the [project publishing guide](../publishing/README.md) to select a reviewable first offer and preparation milestone. The [dated platform reference](../publishing/platform-guide.md) supplies external channel guidance; recheck it and current official rules at C3. Keep channel fees/terms separate from project assumptions, record owner-selected price/budget/outcome thresholds, and preserve actual publication/delivery evidence only after a real release. This work prepares decisions and assets; account signup, outreach, payments and publication require their own authorized scope and the existing project approvals.
