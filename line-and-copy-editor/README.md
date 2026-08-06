# line-and-copy-editor

A [Claude skill](https://www.anthropic.com/news/skills) for combined line editing and copy editing of nonfiction manuscripts in a single sweep — sentence-level prose work plus grammar, consistency, and factual cross-checks. Especially suited to manuscripts that have been through AI-assisted drafting or "humanizer" passes and now need one careful pass to remove machine-prose artifacts, tighten rhythm, and lock down style.

Output is real Word track changes (not a marked-up text file), a running style sheet, and an editorial cover letter — the deliverables a human combined editor would produce.

Part of the [claude-skills](../) collection.

## Why this exists

A pure copy editor fixes grammar and misses prose rhythm. A pure line editor fixes prose and skips factual consistency. A *combined* edit does both, in one sweep, on a manuscript that's structurally sound but stylistically rough. That's a real category of work — EFA calls it "stylistic + copy editing"; some Reedsy listings call it "combined edit" — and it's the right tool when:

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
    └── style-guide-template.md           # template for the running style sheet
```

`SKILL.md` is the operational document. It covers:

- Scope (in / out)
- AI-prose artifacts to watch for — humanizer mechanical glitches, repetitive patterns, em-dash dependency
- Order of operations inside a chunk (compression first, then copy-edits, then fact checks)
- Compression strategy with priority list
- Track changes vs comments
- Style sheet management
- Cross-chapter consistency tracking (names list, facts list, defined-terms list)
- Citation and reference alignment
- Calibration phase
- Quality bar and deliverables
- Default style standards (Chicago, MW, US English)
- Technical reference for producing real Word track changes via docx XML

## How to install

See the [parent README](../README.md#how-to-use-a-skill) for installation across Claude.ai, Claude Code, and other surfaces. The short version for Claude Code:

```bash
cp -r line-and-copy-editor ~/.claude/skills/
```

## Quickstart for a real engagement

1. Read `SKILL.md` end to end before starting.
2. Copy `references/style-guide-template.md` to your working directory and fill in the engagement parameters.
3. Confirm scope, style standard, em-dash convention, target wordcount, and chunk size with the author.
4. Run a calibration pass on 1,500–2,500 words. Get feedback. Adjust.
5. Work through the manuscript chunk by chunk: compression first, copy-edits second, facts last. Update the style sheet on every chunk.
6. Final sweep for citation and reference alignment after all chunks are edited.
7. Deliver the manuscript with track changes, the cover letter, the style sheet, and the names/facts lists.

## What this skill is not

- Not a developmental edit. It does not restructure chapters or add arguments.
- Not a proofread. It's heavier than that and does prose-level work.
- Not a ghostwrite. Voice preservation is a hard constraint.
- Not an AI-pass tool. If your manuscript already has machine-prose artifacts, running it through another generation pass compounds the problem. This skill edits by hand, surgically, using track changes the author can accept or reject one by one.

## Acknowledgments

This skill was inspired by and adapted from two prior projects, both used under MIT license:

- [@lfurze/claude-skills](https://github.com/lfurze/claude-skills) — docx XML editing technical reference and multi-pass workflow structure.
- [@felipelobomotta-blip/book-genesis-v4](https://github.com/felipelobomotta-blip/book-genesis-v4) — editor role definition, scope framing, AI-prose artifact awareness, and quality-bar conventions.

See the [parent README](../README.md#acknowledgments) for the full attribution and required copyright notices.

## License

MIT — see [LICENSE](../LICENSE) at the repo root.
