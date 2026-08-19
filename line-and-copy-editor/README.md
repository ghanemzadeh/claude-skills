# line-and-copy-editor

A [Claude skill](https://www.anthropic.com/news/skills) for combined line editing and copy editing of nonfiction manuscripts in a single sweep: sentence-level prose work plus grammar, consistency, and factual cross-checks. It is built for manuscripts that have been through AI-assisted drafting or "humanizer" passes and need one careful pass to remove machine-prose artifacts, tighten rhythm, and lock down style.

Output is real Word track changes (an actual `.docx` the author can review), a running style sheet, and an editorial cover letter: the deliverables a human combined editor would produce.

Part of the [claude-skills](../) collection.

## Why this exists

A pure copy editor fixes grammar and misses prose rhythm. A pure line editor fixes prose and skips factual consistency. A combined edit does both in one sweep, on a manuscript that's structurally sound but stylistically rough. The EFA calls this "stylistic + copy editing"; some Reedsy listings call it a "combined edit." It's the right tool when:

- You have a long-form manuscript that's been AI-drafted or AI-rewritten and reads unevenly
- You need to cut wordcount by 10–15% without losing arguments
- You need final SPAG, consistency, and voice work in one pass before proofreading
- You need every recurring style decision documented for future revisions or sequels

## What's in this folder

```
line-and-copy-editor/
├── SKILL.md                              # the skill itself
├── README.md                             # this file
└── references/
    ├── style-guide-template.md           # template for the running style sheet
    ├── ai-prose-patterns.md              # catalog of 36 machine-drafting patterns
    └── pre-delivery-checklist.md         # pass/fail self-check run before each chunk ships
```

`SKILL.md` is the operational document: scope, the no-fabrication rule, order of operations inside a chunk (compression first, then copy edits, then fact checks), compression strategy, track changes vs comments, style sheet management, cross-chapter consistency tracking, citation alignment, the calibration phase, quality bar, deliverables, default standards (Chicago 18th, Merriam-Webster, US English), and a technical reference for producing real Word track changes via docx XML.

`references/ai-prose-patterns.md` is the pattern catalog: 36 patterns across six groups, each with trigger words, a default action (track change, comment, cover-letter note, or leave), and a dose budget where a pattern is only a problem in aggregate. It merges the humanizer pattern set with the editing principles from no-ai-slop, adapted for surgical track-changes work instead of rewriting, and adds the mechanical artifacts that humanizer passes themselves leave behind. Since v2.1.0 the skill also carries document-level guidance on editing toward human prose: sentence and paragraph variance, short endings, register match in insertions, and specificity via author query.

`references/pre-delivery-checklist.md` is the gate each chunk passes before delivery: voice, proportionality, no new slop in the insertions, no fabricated facts, dose budgets, and docx mechanics.

## How to install

See the [parent README](../README.md#how-to-use-a-skill) for installation across Claude.ai, Claude Code, and other surfaces. The short version for Claude Code:

```bash
cp -r line-and-copy-editor ~/.claude/skills/
```

## Quickstart for a real engagement

1. Read `SKILL.md` end to end before starting.
2. Read `references/ai-prose-patterns.md`; it drives the prose layer of the edit.
3. Copy `references/style-guide-template.md` to your working directory and fill in the engagement parameters.
4. Confirm scope, style standard, em-dash convention, target wordcount, and chunk size with the author.
5. Run a calibration pass on 1,500–2,500 words. Get feedback. Adjust.
6. Work through the manuscript chunk by chunk: compression first, copy edits second, facts last. Run the pre-delivery checklist on every chunk and update the style sheet as you go.
7. Final sweep for citation and reference alignment after all chunks are edited.
8. Deliver the manuscript with track changes, the cover letter, the style sheet, and the names and facts lists.

## What this skill is not

- A developmental edit. It does not restructure chapters or add arguments.
- A proofread. It's heavier than that and does prose-level work.
- A ghostwrite. Voice preservation is a hard constraint.
- An AI-pass tool. If your manuscript already has machine-prose artifacts, another generation pass compounds the problem. This skill edits by hand, surgically, using track changes the author can accept or reject one by one.

## Acknowledgments

This skill was adapted from prior projects, all used under MIT license:

- [@lfurze/claude-skills](https://github.com/lfurze/claude-skills): docx XML editing technical reference and multi-pass workflow structure.
- [@felipelobomotta-blip/book-genesis-v4](https://github.com/felipelobomotta-blip/book-genesis-v4): editor role definition, scope framing, AI-prose artifact awareness, and quality-bar conventions.
- [@blader/humanizer](https://github.com/blader/humanizer) (v2.11.2): the pattern set underlying `references/ai-prose-patterns.md`, itself based on Wikipedia's [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) guide.
- [@petergyang/no-ai-slop](https://github.com/petergyang/no-ai-slop) (v1.0.6): editing principles (minimum effective edits, proportionality, the portability test), word lists, and the eval-checklist approach behind `references/pre-delivery-checklist.md`.

The "Editing toward human prose" section and the human-writing checklist items draw on published research from Pangram Labs ([pangram.com/blog](https://www.pangram.com/blog) and the [Pangram substack](https://pangram.substack.com)) about document-level differences between human and AI prose. Cited as research; no code or text is reused.

See the [parent README](../README.md#acknowledgments) for the full attribution and copyright notices.

## License

MIT: see [LICENSE](../LICENSE) at the repo root.
