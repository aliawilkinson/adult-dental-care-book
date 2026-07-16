# Draft 1 Paginated Cloud Workflow

Use this workflow when one full-book cloud task produces only a thin scaffold or stops too early.

For the exact overnight run protocol, start with:

```text
tasks/how-to-run-overnight-book-workflow.md
```

That file is the current operational guide. This paginated workflow is the fallback when the overnight run still leaves thin sections.

## Branch Strategy

Use one review branch for the full Draft 1 sequence:

```text
codex/overnight-draft-1
```

`main` already contains the scaffold and workflow materials. Continue expansion on `codex/overnight-draft-1` until the manuscript is genuinely readable. Run each page as a separate Codex cloud task or follow-up on the same branch. Do not merge to `main` as Draft 1 until Page 4 is complete and reviewed.

## Page Sequence

The current controlling outline is `outline.md`. The page prompts should follow that outline, even if older prompt text uses previous chapter numbers.

1. `tasks/paginated-draft-1/page-01-foundation.md`
   - Foreword
   - Introduction
   - Chapters 1-6
2. `tasks/paginated-draft-1/page-02-prevention-cosmetic.md`
   - Chapters 7-13
3. `tasks/paginated-draft-1/page-03-dentist-long-term-reference.md`
   - Chapters 14-17
   - Quick Reference
   - Product Guide
   - FAQ
   - Appendix seeds
4. `tasks/paginated-draft-1/page-04-integrate-review.md`
   - Assemble full manuscript
   - Trim repetition
   - Voice pass
   - Source-needs pass
   - Final summary

## Recommended Cadence

Run the overnight workflow first if you want a single long attempt. In the morning, inspect the output before launching a paginated follow-up.

If a page is too thin, rerun that page with a stronger expansion instruction before moving on. Do not let Codex proceed just because files exist.

## Completion Standard

Draft 1 is not complete until:

- every outline bullet has been covered or explicitly moved
- every chapter has substantive prose rather than scaffold notes
- `book/full-manuscript.md` is assembled
- each chapter has a word count and readiness rating in `reviews/final-summary.md`
- unresolved claims are marked rather than invented
- the manuscript sounds like Alia, not a generic dental-office blog

Use length as a guardrail, not a goal. Short is acceptable when complete. Generic and thin is not.
