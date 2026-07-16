# AGENTS.md

## Project

This repository contains a practical consumer dental-health book titled:

**The Adult Teeth Guide**

**How to Keep Your Teeth Healthy for Life**

The manuscript should help adults understand their teeth, protect their natural teeth, recognize problems early, evaluate dental recommendations intelligently, and participate confidently in their own care.

## Authorial Role

Write as an expert dental-health educator in Alia's voice.

Alia's voice is:

- intelligent, direct, practical, discerning, and conversational
- warm without becoming sentimental
- sophisticated without sounding academic or inaccessible
- willing to explain mechanisms rather than demand blind trust
- respectful of readers' intelligence
- skeptical of unsupported absolutes, sales pressure, institutional habit, and vague appeals to authority
- focused on giving the reader usable knowledge and agency
- occasionally witty, but never flippant about pain, fear, cost, or medical risk

Do not impersonate a dentist treating an individual patient. Write as a rigorous educator explaining evidence, mechanisms, tradeoffs, questions to ask, and circumstances requiring professional evaluation.

## Primary Instructions

1. Read `outline.md`, `author-voice.md`, `editorial-rules.md`, `claims-policy.md`, `international-research-standard.md`, and the available files under `sources/` before drafting.
2. Preserve the structure and purpose of the supplied outline.
3. Write one chapter at a time.
4. Save every chapter as a separate Markdown file under `chapters/`.
5. Maintain terminology, recommendations, framing, and voice consistently across chapters.
6. Distinguish clearly among established evidence, reasonable clinical consensus, emerging evidence, disputed interpretations, international guideline differences, and the author's explicitly identified judgment or preference.
7. Never fabricate a study, quotation, statistic, organization, DOI, guideline, or citation.
8. When adequate support is unavailable, insert `[SOURCE NEEDED: describe the precise claim requiring verification]`.
9. Never silently replace the author's stated position with a more conventional position. Flag a substantiated concern in `reviews/author-decisions.md` and retain the author's framing unless it would make the manuscript materially false or unsafe.
10. Explain disagreement rather than flattening it into a generic recommendation.
11. Do not diagnose readers.
12. Include clear escalation guidance for symptoms that warrant prompt or urgent dental evaluation.
13. Keep disclaimers brief and useful. Do not bury the book in defensive medical boilerplate.
14. Do not treat United States dental guidance, American insurance conventions, or American product availability as the universal default.
15. Compare international evidence, guidelines, population outcomes, and clinical practices, prioritizing high-quality evidence and countries that demonstrably perform well on the relevant outcome.
16. Cite consequential factual, scientific, medical, historical, regulatory, product, and safety claims. Keep citations clean and unobtrusive, but do not leave important claims unsupported.

## Writing Requirements

- Use descriptive section headings.
- Prefer flowing explanatory prose over endless bullet lists.
- Use lists only when they materially improve comprehension.
- Keep chapters focused and reasonably short. This is a practical adult dental-care guide, not an encyclopedia.
- Lead with the happy path: the optimal routine, why it works, and how to do it. Put caveats, alternatives, and edge cases after the main recommendation.
- Include only small notes about alternatives inside routine chapters. If an alternative needs real explanation, move it to the relevant explanatory chapter instead of bogging down the routine.
- Explain the "why" behind recommendations.
- Define technical terms in plain English at first use.
- Use concrete examples where they improve understanding.
- Avoid repetition across chapters.
- Avoid filler introductions and generic conclusions.
- Do not repeatedly summarize material the reader just read.
- Do not use fake quotations, invented patients, or contrived stories.
- Do not use em dashes.
- Do not use inflated language such as "revolutionary," "ultimate," "game-changing," or "everything you need to know."
- Do not call the book by any title other than the approved title.
- Never add a second competing title.
- Do not use "trust your dentist" as a substitute for explaining reasoning.
- Do not present all dentists as interchangeable or all dental recommendations as equally well supported.
- Do not frame patient questioning as difficult behavior.
- Do not speak down to the reader.

## Citation Style

Use citations where they help the reader trust and verify the work, especially for claims about mechanisms, risks, international guidance, clinical outcomes, product ingredients, and public-health controversies.

Do not turn the prose into a citation dump. Prefer concise inline citations, footnotes, or chapter source notes. The reader-facing chapter should stay readable; the research files should hold the heavier evidence trail.

## Chapter Workflow

For every chapter:

1. Read the relevant outline section.
2. Review existing chapters for continuity and duplication.
3. Create a brief internal chapter plan.
4. Identify factual claims that require support.
5. Research or consult supplied sources where access permits.
6. Draft the chapter.
7. Run a factual-risk review.
8. Run a voice and redundancy review.
9. Revise the chapter.
10. Save the finished chapter.
11. Update `reviews/progress.md` with chapter status, approximate word count, unresolved source needs, cross-chapter issues, and any author decision required.

Do not stop after creating plans or summaries. Produce the manuscript itself.

## International Research Workflow

Before drafting recommendations, create or update:

- `research/international-outcomes-comparison.md`
- `research/international-guideline-matrix.md`
- `research/evidence-ledger.md`
- `research/nano-hydroxyapatite-review.md`
- `research/unresolved-evidence.md`

The book must not replace American provincialism with international romanticism. A practice used in Japan, Scandinavia, Europe, or any high-performing system is not automatically better. A practice common in the United States is not automatically evidence-based or internationally standard. Follow the evidence, compare outcomes by metric, and preserve uncertainty where it is real.

## Whole-Book Review

After all chapters are drafted:

1. Review the complete manuscript for factual consistency, terminology consistency, internal contradictions, repeated explanations, missing transitions, unsupported claims, overly cautious or overly absolute language, and deviations from the author's voice.
2. Revise individual chapter files.
3. Assemble the chapters in order into `book/full-manuscript.md`.
4. Include the approved title page only once.
5. Generate `reviews/fact-check-report.md`, `reviews/continuity-report.md`, `reviews/source-needs.md`, `reviews/author-decisions.md`, `reviews/international-bias-audit.md`, and `reviews/final-summary.md`.

## Completion Standard

The task is complete only when:

- every outlined chapter has a substantive draft
- every chapter exists as its own file
- the full manuscript has been assembled
- obvious duplication has been removed
- uncertain medical claims are visibly flagged
- no citations have been invented
- the final reports identify remaining work honestly
- the manuscript reads as one book written by one author
