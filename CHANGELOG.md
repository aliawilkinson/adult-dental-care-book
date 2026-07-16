# Changelog

All notable changes to this project will be documented in this file.

This project uses Semantic Versioning for repository and manuscript workflow milestones.

## [0.1.3] - 2026-07-16

### Added

- Added a paginated Draft 1 cloud workflow for expanding the manuscript in bounded chapter groups.
- Added separate prompts for foundation, prevention/cosmetic, dentist/long-term/reference, and integration/review passes.

### Changed

- Clarified the recommended Draft 1 strategy: use multiple branch-preserving cloud tasks instead of one oversized full-book expansion run.

## [0.1.2] - 2026-07-16

### Added

- Added the final overnight Draft 1 priority instruction directly to the Codex cloud task prompt.
- Added explicit guidance to run the overnight manuscript work on `codex/overnight-draft-1` instead of `main`.

### Changed

- Clarified that Draft 1 should prioritize full-book coverage, practical happy-path chapters, verified citations, and honest source flags over exhaustive research matrices.

## [0.1.1] - 2026-07-16

### Added

- Added explicit citation requirements for consequential dental, scientific, product, historical, regulatory, and safety claims.
- Added a dedicated outline chapter for fluoride, nano-hydroxyapatite, water fluoridation, comparative mechanisms, evidence, and safety questions.
- Added happy-path drafting rules so routine chapters stay clear, practical, and not too long.

### Changed

- Clarified that the daily routine should stay nHA-forward and simple, with deeper fluoride/nHA nuance moved into its own chapter.
- Updated editorial guidance so chapters lead with what to do and why before alternatives, caveats, or edge cases.

## [0.1.0] - 2026-07-16

### Added

- Established the book repository structure for **The Adult Teeth Guide: How to Keep Your Teeth Healthy for Life**.
- Added durable project instructions in `AGENTS.md`.
- Added the approved outline in `outline.md`.
- Added voice, editorial, claims, and international research standards.
- Added the nHA-forward dental care regimen as a source copy artifact.
- Added research tracking files for claim mapping, international outcomes, international guideline comparison, evidence ledger, unresolved evidence, and nano-hydroxyapatite review.
- Added review tracking files for progress, author decisions, source needs, manuscript planning, and international bias auditing.
- Added the paste-ready Codex cloud task prompt for a full international-first manuscript drafting run.
- Added initial manuscript assembly placeholder at `book/full-manuscript.md`.
- Added `.superpowers/` to `.gitignore` for local Codex brainstorming artifacts.

### Changed

- Updated `README.md` from a short repo description into a working repository map.

### Notes

- This is a scaffold and workflow release, not a complete manuscript release.
- The next major milestone is a complete first-draft manuscript with research files and review reports populated.
