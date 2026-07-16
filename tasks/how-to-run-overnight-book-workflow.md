# How To Run The Overnight Book Workflow

Use this when the goal is to wake up to an actual useful manuscript, not a technically complete but thin scaffold.

## Current Branch Reality

The working Draft 1 branch is:

```text
codex/overnight-draft-1
```

`main` has already received the scaffold and paginated workflow. Continue manuscript expansion on `codex/overnight-draft-1` until the book is genuinely readable. Do not start over on a fresh branch unless the existing branch becomes unusable.

## What "Actual Book" Means Here

Do not optimize for length by padding. Optimize for coverage and usefulness.

A chapter is substantive when it:

1. Covers every bullet in `outline.md` for that chapter, or explicitly explains in `reviews/final-summary.md` why a bullet moved elsewhere.
2. Opens with the happy path: what to do, why it works, and how to do it.
3. Explains the mechanism in plain language.
4. Includes practical adult examples without fake patient stories.
5. Flags symptoms that should escalate to prompt or urgent dental evaluation where relevant.
6. Separates evidence, clinical consensus, emerging evidence, disputed claims, and author preference.
7. Uses `[SOURCE NEEDED: precise claim]` or `[PRIMARY SOURCE VERIFICATION REQUIRED]` instead of inventing citations.
8. Sounds like Alia: direct, warm, skeptical, practical, and not like a dental-office blog.

A chapter is still a scaffold when it mostly says what the chapter will cover, repeats generic foundation language, or leaves outline bullets unaddressed.

## Length Guidance Without Padding

Short is fine when the chapter is complete. Thin is not fine.

Use these as guardrails, not padding instructions:

- Foreword and introduction: usually 500-1,500 words each.
- Main chapters: usually 1,200-2,800 words each.
- Quick reference: as short as possible while genuinely useful.
- Full manuscript: likely 25,000-45,000 words for a practical first draft.

If the manuscript is under 25,000 words, it can still be acceptable only if `reviews/final-summary.md` gives a chapter-by-chapter reason why the outline is fully covered without padding. If any main chapter is under 1,000 words, continue expanding unless it is intentionally short and justified in the final summary.

## Recommended Overnight Run

Run one Codex cloud task on the current branch with the prompt below.

```text
You are on `codex/overnight-draft-1`. The current manuscript is still scaffold-level. Expand it into a real practical Draft 1 using `outline.md` as the controlling outline.

Do not create placeholder chapters. Do not stop after planning. Do not mark the manuscript complete because files exist. The goal is coverage and usefulness, not padding.

Read first:
- AGENTS.md
- outline.md
- author-voice.md
- editorial-rules.md
- claims-policy.md
- international-research-standard.md
- cheat-sheets/dental-care-regimen.md
- all current chapter files
- reviews/final-summary.md
- reviews/source-needs.md
- research/unresolved-evidence.md

Then rewrite and expand chapters in this order:
1. Foreword and Introduction, only if they need smoothing after the latest outline correction.
2. Part I: Chapters 1-3.
3. Part II: Chapters 4-6.
4. Part III: Chapters 7-9.
5. Part IV: Chapters 10-13.
6. Part V: Chapters 14-15.
7. Part VI: Chapters 16-17.
8. Part VII: Quick Reference, Product Guide, FAQ, Appendix seeds, and Bonus Downloads.

For every chapter:
- Cover every outline bullet.
- Lead with the useful recommendation or concept.
- Explain why it works.
- Keep the tone practical and adult.
- Do not lecture about habits. Explain mechanisms, mitigation, and what quitting changes.
- Avoid fake stories and generic AI intros/conclusions.
- Do not use em dashes.
- Do not invent citations.
- Add `[SOURCE NEEDED: precise claim]` where verification is incomplete.

Important structure decisions:
- Use the approved title only: The Adult Teeth Guide.
- Keep the approved subtitle: How to Keep Your Teeth Healthy for Life.
- Treat "Everything you wanted to know about keeping your teeth healthy and strong for life" as positioning copy, not a competing title.
- Use the user's latest `outline.md` chapter sequence as controlling.
- Fluoride and nHA should be explained inside Chapter 5 or a clearly labeled tool/reminalization subsection unless the outline is explicitly revised again.

Before stopping:
1. Reassemble `book/full-manuscript.md` from chapter files.
2. Run a word-count script across `chapters/*.md`.
3. Run a coverage check against `outline.md` and list any missed bullets.
4. Update `reviews/progress.md` with word count, readiness, source needs, and cross-chapter issues.
5. Update `reviews/final-summary.md` with:
   - total chapter word count
   - word count per chapter
   - which chapters are strong, usable, skeletal, or unresolved
   - any outline bullets still missing
   - what still needs source verification
   - whether this is a real Draft 1 or still scaffold-level

Completion gate:
If any main chapter is still generic or under 1,000 words without a clear reason, continue expanding it.
If the total manuscript is under 25,000 words, continue unless the final summary proves the outline is fully covered without padding.
If the final summary would honestly say "scaffold," keep working.
```

## If The Task Still Finishes Too Fast

Do not merge it as Draft 1. Run the next paginated task for the weakest section:

- `tasks/paginated-draft-1/page-01-foundation.md`
- `tasks/paginated-draft-1/page-02-prevention-cosmetic.md`
- `tasks/paginated-draft-1/page-03-dentist-long-term-reference.md`
- `tasks/paginated-draft-1/page-04-integrate-review.md`

Tell Codex exactly which chapters were thin and require expansion. Use chapter word counts and missing outline bullets as the enforcement mechanism.

## Morning Review Checklist

When you wake up, check:

1. Does `reviews/final-summary.md` say "real Draft 1" or "scaffold"?
2. Are any main chapters under 1,000 words?
3. Did it update `book/full-manuscript.md`?
4. Are `[SOURCE NEEDED]` markers precise rather than vague?
5. Does the prose sound like Alia, or like a dental website trying to improve SEO?
6. Are the outline bullets actually covered?

If the answer is no, run the relevant paginated task instead of accepting the manuscript as done.
