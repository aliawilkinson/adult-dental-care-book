# The Adult Teeth Guide

## How to Keep Your Teeth Healthy for Life

I realized I knew nothing about adult dental care but wanted perfect teeth, and after four cavities I went on a dental journey. I am turning it into a book because I want to keep it to read it as a reminder. I also need a cheat sheet for my bathroom mirror in the form of an attractive poster. I think this is something others could benefit from too.

This repository treats the book like a software project: durable instructions, source tracking, chapter files, review reports, and a final assembled manuscript.

Current version: `0.1.3`

## Repository Map

- `VERSION`: current semantic version.
- `CHANGELOG.md`: version history.
- `AGENTS.md`: standing instructions for Codex and future agents.
- `outline.md`: approved book structure.
- `author-voice.md`: voice samples and style reference.
- `editorial-rules.md`: writing rules and framing.
- `claims-policy.md`: evidence and safety policy for dental claims.
- `international-research-standard.md`: required international evidence and outcomes workflow.
- `cheat-sheets/`: author-facing routine and quick-reference copy.
- `sources/`: source index and reference notes.
- `research/`: claim maps and research work.
- `chapters/`: one Markdown file per chapter.
- `reviews/`: progress, source needs, editorial reports, and author decisions.
- `book/full-manuscript.md`: assembled manuscript.
- `releases/`: release notes by version.
- `tasks/overnight-codex-cloud-task.md`: prompt for a long-running Codex cloud drafting task.

## Working Rule

Draft the book one chapter at a time, keep claims source-aware, compare international evidence and outcomes before making major recommendations, and preserve the author's direct, practical, non-institutional voice.

## Development Branch Sync

When `main` changes, `.github/workflows/sync-main-to-development-branches.yml` opens or refreshes reviewable sync pull requests for same-repository branches beginning with `claude/`, `codex/`, `dev/`, `feature/`, or `fix/` that have an open pull request into `main`. The workflow never merges directly into a development branch. Closed, merged, abandoned, and fork-based branches are ignored. Conflicts are reported for manual resolution.
