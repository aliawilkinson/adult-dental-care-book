# Draft 1 Expansion Codex Cloud Task

Paste this task into a Codex cloud task connected to this repository.

## Launch Setup

Use the existing branch/PR:

```text
codex/overnight-draft-1
```

Do not start a new scaffold branch. Do not work directly on `main`. Enable internet access in the Codex cloud environment before starting, because this task still requires source verification when making consequential medical, scientific, product, regulatory, or safety claims.

## Task

The current branch is NOT a complete Draft 1. It is only a thin scaffold.

Your task is to expand it into a real, readable Draft 1 manuscript.

Do not create more placeholder files. Do not merely summarize. Do not stop after planning. Do not mark the book complete until the manuscript is substantially drafted.

Primary goal:
Expand every chapter file under `chapters/` into substantive prose while preserving the approved outline, title, author voice, happy-path practical style, and citation rules.

Target length:

- Total chapter word count target: 40,000-60,000 words.
- Main chapters should generally be 1,800-3,500 words each.
- Foreword, introduction, and quick reference may be shorter, but should still be useful.
- No substantive chapter may remain under 1,200 words unless you explicitly justify why in `reviews/final-summary.md`.

Workflow:

1. Read `AGENTS.md`, `outline.md`, `author-voice.md`, `editorial-rules.md`, `claims-policy.md`, `international-research-standard.md`, and current chapter files.
2. Treat the existing chapter files as scaffolds to expand, not finished chapters.
3. Expand chapters one by one into finished Draft 1 prose.
4. Prioritize writing the book over filling research matrices.
5. Cite consequential claims when reliable sources are available.
6. If verification cannot be completed, keep the passage only if responsibly qualified and add `[SOURCE NEEDED: precise claim]` or `[PRIMARY SOURCE VERIFICATION REQUIRED]`.
7. Do not invent citations.
8. Keep the daily routine happy-path and practical.
9. Put deeper debates, especially fluoride vs. nHA, in the dedicated chapter.
10. Preserve Alia's voice: smart, direct, practical, non-institutional, not dental-office blog prose.

Completion gate:
Before stopping, run a word-count check across `chapters/*.md`.

If total chapter word count is under 40,000 words, continue expanding.

If any main chapter is under 1,200 words, continue expanding or explain clearly in `reviews/final-summary.md` why it is intentionally short.

Then assemble `book/full-manuscript.md` from the chapter files.

Update:

- `reviews/final-summary.md`
- `reviews/source-needs.md`
- `reviews/author-decisions.md`
- `reviews/progress.md`

Final summary must state:

- total chapter word count
- word count per chapter
- which chapters are strong, usable, skeletal, or unresolved
- what still needs source verification
- whether this is a real Draft 1 or still only a scaffold
