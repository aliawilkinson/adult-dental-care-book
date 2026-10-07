# Dependency maintenance audit: C2/C5

Reviewed 2026-10-06 America/Los_Angeles; verified 2026-10-07T03:32:30.924744+00:00. Source: `5f80f5d55942c72b3026ce3578d444013e4b47c9`. Default branch: `main`. Default SHA: `a7c862b82520bdf113c00eeeb565878168712b62`. Prepared by Codex for the requested Projects-folder dependency audit.

## Evidence and decision

The two existing workflows reference checkout/upload actions plus shared release, asset-publishing and branch-sync workflows. The release-please JSON files store release/version configuration, not installable package dependencies.

Added `.github/dependabot.yml` with one `github-actions` entry for `/`, a weekly interval and a five-PR limit. Existing action/workflow refs are unchanged. No existing Dependabot policy was present to replace.

[Dependabot configuration](../../../.github/dependabot.yml)

The audit included hidden `.github` files, tracked package/lock/build manifests and dependency-install/import statements in existing tooling/workflows. No inline `pip install` needing extraction into a requirements file was found. Original active working branches were checked as well as the freshly fetched default; unpublished work and untracked source assets were preserved. The documentation branch contains the latest fetched default as an ancestor where a Git repository exists.

## Verification

Ruby 4.0.7; Psych 5.3.1 parsed the config and all 2 workflow YAML files. Semantic checks require version 2, the Actions ecosystem, root `/`, weekly schedule, a positive limit of five and no unexpected update options. Found 5 referenced actions/reusable workflows.

[GitHub's Actions update guidance](https://docs.github.com/en/code-security/how-tos/secure-your-supply-chain/secure-your-dependencies/auto-update-actions) covers referenced actions and reusable workflows. Its [configuration reference](https://docs.github.com/en/code-security/reference/supply-chain-security/dependabot-options-reference) requires the `/` directory for Actions and supports weekly schedules. Configuration validation is local; actual Dependabot activation/update success after merge requires GitHub's update logs. Upstream shared-workflow internals remain maintained in their owning repository.

## GitHub settings observation

A read-only `GET repos/aliawilkinson/adult-dental-care-book/automated-security-fixes` at `2026-10-07T03:33:19.365684+00:00` returned `enabled: false`, `paused: false`. No repository setting was changed. This observation is separate from the proposed weekly version-update configuration; these Actions-only repositories have no package manifest from which to claim package security-update coverage. Actual post-merge scan success remains unverified.

## Maintenance and signoff

On adding a workflow, package manager or build/export dependency, repeat this inventory and add the correct ecosystem at each real manifest root. Keep runtime/toolchain maintenance separate when no supported manifest exists. Review proposed dependency changes through the usual branch/PR and applicable content/release checks; this milestone performs no dependency upgrade, automatic merge, release or publication.

Signoff: **ship the scoped configuration/audit for review**. Applicable config becomes effective through the normal default-branch merge; post-merge scan success is **unverified**. For N/A scopes, the trigger for another review is a new supported manifest, external install or workflow. No provider setting, credentials, manuscript or application source changed.
