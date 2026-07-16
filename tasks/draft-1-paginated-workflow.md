# Draft 1 Paginated Cloud Workflow

Use this workflow when one full-book cloud task produces only a thin scaffold or stops too early.

## Branch Strategy

Use one review branch for the full Draft 1 sequence:

```text
codex/overnight-draft-1
```

Run each page as a separate Codex cloud task or follow-up on the same branch. Do not merge to `main` until Page 4 is complete and reviewed.

## Page Sequence

1. `tasks/paginated-draft-1/page-01-foundation.md`
   - Foreword
   - Introduction
   - Chapters 1-6
2. `tasks/paginated-draft-1/page-02-prevention-cosmetic.md`
   - Chapters 7-13
3. `tasks/paginated-draft-1/page-03-dentist-long-term-reference.md`
   - Chapters 14-18
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

Run Page 1 first. In the morning, inspect the output before launching Page 2. If Page 1 is too thin, rerun Page 1 with a stronger expansion instruction before moving on.

## Completion Standard

Draft 1 is not complete until:

- every outlined chapter has substantive prose
- `book/full-manuscript.md` is assembled
- each chapter has a word-count and readiness rating in `reviews/final-summary.md`
- unresolved claims are marked rather than invented
- the manuscript sounds like Alia, not a generic dental-office blog
