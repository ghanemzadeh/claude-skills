# claude-skills

A collection of [Claude skills](https://www.anthropic.com/news/skills) for serious writing and editing tasks. Each skill lives in its own folder with a `SKILL.md` file plus any references it needs.

## Skills

| Skill | What it does |
|---|---|
| [`line-and-copy-editor`](./line-and-copy-editor) | Combined line + copy editing for nonfiction manuscripts in a single sweep: sentence-level prose work plus grammar, consistency, and factual cross-checks. Built for manuscripts that have been through AI-assisted drafting or "humanizer" passes. Produces real Word track changes, a running style sheet, and an editorial cover letter. Ships with a 36-pattern catalog of machine-drafting tells and a pre-delivery checklist. |

Each skill in this repo is self-contained; install only the ones you need.

## How to use a skill

There are several ways to load a skill into Claude depending on the surface you're using.

**Claude.ai (web / desktop / mobile)**: upload the skill folder (e.g. `line-and-copy-editor/`) from the skills interface in supported plans, then describe your task and Claude will follow the workflow. For up-to-date instructions, see Anthropic's documentation at <https://support.claude.com>.

**Claude Code**: copy the skill folder into your Claude Code skills directory:

```bash
# Clone this repo, then copy or symlink the skill you want
git clone https://github.com/ghanemzadeh/claude-skills.git
cp -r claude-skills/line-and-copy-editor ~/.claude/skills/

# Or symlink, so updates flow through
ln -s "$(pwd)/claude-skills/line-and-copy-editor" ~/.claude/skills/line-and-copy-editor
```

**As context in any Claude conversation**: paste the contents of a skill's `SKILL.md` into your conversation as context. Less elegant, but it works anywhere Claude is available.

## Repository layout

```
.
├── README.md                              # this file
├── LICENSE                                # MIT
└── line-and-copy-editor/
    ├── SKILL.md                           # the skill itself
    ├── README.md                          # skill-specific docs
    └── references/
        ├── style-guide-template.md        # running style sheet template
        ├── ai-prose-patterns.md           # 36-pattern machine-drafting catalog
        └── pre-delivery-checklist.md      # per-chunk pass/fail self-check
```

## Acknowledgments

The `line-and-copy-editor` skill was adapted from prior projects, all used under MIT license:

**[@lfurze/claude-skills](https://github.com/lfurze/claude-skills)**: provided the docx XML editing technical reference and the multi-pass editing workflow structure.

**[@felipelobomotta-blip/book-genesis-v4](https://github.com/felipelobomotta-blip/book-genesis-v4)**: provided framing for the editor's role definition, scope boundaries, AI-prose artifact awareness, and quality-bar conventions.

**[@blader/humanizer](https://github.com/blader/humanizer)** (v2.11.2): provided the AI-writing pattern set adapted into `references/ai-prose-patterns.md`, itself based on Wikipedia's [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) guide.

**[@petergyang/no-ai-slop](https://github.com/petergyang/no-ai-slop)** (v1.0.6): provided editing principles (minimum effective edits, proportionality, the portability test), word lists, and the eval-checklist approach adapted into `references/pre-delivery-checklist.md`.

The skill's "Editing toward human prose" section also draws on published research from Pangram Labs ([pangram.com/blog](https://www.pangram.com/blog) and the [Pangram substack](https://pangram.substack.com)) about document-level differences between human and AI prose. This is a research citation, not reused code or text, so it sits outside the MIT notices below.

All four are released under the MIT License. The required copyright notice and permission text:

```
MIT License

Copyright (c) lfurze
Copyright (c) Felipe Lobo Motta
Copyright (c) 2025 Siqi Chen (blader/humanizer)
Copyright (c) 2026 Peter Yang (petergyang/no-ai-slop)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## License

MIT: see [LICENSE](LICENSE) for the full text. Each skill in this repo is released under the same license unless otherwise noted in the skill's own folder.

## Contributing

Issues and PRs welcome. If you have a skill you'd like to add, open an issue first to discuss whether it fits the scope of this collection.
