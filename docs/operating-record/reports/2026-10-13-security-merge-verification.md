# Merge verification follow-up — 2026-10-13 America/Los_Angeles

Owner explicitly requested merging the prepared changes after review. This approves the Mermaid 12 / KaTeX 0.18 compatibility proposal; the earlier hold remains historical evidence.

Reviewed head 8418a4c7437d73515b311a948364809cd5645dd4, base 8d73db04fb68d9b1df37e9736c06ffcd46614a0c. Full local checkout reconstructed from all Git blobs; its exact tree matches the GitHub candidate. Frozen npm install with scripts disabled, all five tests (zero skips), npm run check (14 files, three diagrams, 78 links), and complete dependency graph pass. The four tools have identical manifests/locks; fresh candidate audit has zero findings versus two low entries on exact base. All review comments/submissions and inline threads were read; none exist on this proposal.

A remaining push-triggered release workflow could invoke release-please and package manuscript assets during routine integration. Consistent with the owner's October 7 approval of explicitly requested source releases, this follow-up removes only the push trigger. Manual release, packaging, permissions and existing release conditions are preserved. YAML parsing confirms workflow_dispatch is the sole trigger. No hosted PR verification workflow exists for this documentation tool; zero PR checks are not represented as a hosted pass.

Signoff: SHIP source after final unchanged-head/base and normal GitHub merge checks. Publication/deployment remains a separate owner action. No manuscript, private source or existing immutable release was changed.
