# claude-skills

A collection of [Claude skills](https://www.anthropic.com/news/skills) for editorial, writing, and product work. Each skill lives in its own folder with a `SKILL.md` file plus any references it needs.

## Skills

| Skill | What it does |
|---|---|
| [`line-and-copy-editor`](./line-and-copy-editor) | Combined line + copy editing for nonfiction manuscripts in a single sweep — sentence-level prose work plus grammar, consistency, and factual cross-checks. Especially suited to manuscripts that have been through AI-assisted drafting or "humanizer" passes. Produces real Word track changes, a running style sheet, and an editorial cover letter. |

More skills will be added over time. Each skill in this repo is self-contained — install only the ones you need.

## How to use a skill

There are several ways to load a skill into Claude depending on the surface you're using.

**Claude.ai (web / desktop / mobile)** — upload the skill folder (e.g. `line-and-copy-editor/`) from the skills interface in supported plans, then describe your task and Claude will follow the workflow. For up-to-date instructions, see Anthropic's documentation at <https://support.claude.com>.

**Claude Code** — copy the skill folder into your Claude Code skills directory:

```bash
# Clone this repo, then copy or symlink the skill you want
git clone https://github.com/<your-username>/claude-skills.git
cp -r claude-skills/line-and-copy-editor ~/.claude/skills/

# Or symlink, so updates flow through
ln -s "$(pwd)/claude-skills/line-and-copy-editor" ~/.claude/skills/line-and-copy-editor
```

**As context in any Claude conversation** — paste the contents of a skill's `SKILL.md` into your conversation as context. Less elegant but works anywhere Claude is available.

## Repository layout

```
.
├── README.md                              # this file
├── LICENSE                                # MIT
└── line-and-copy-editor/
    ├── SKILL.md                           # the skill itself
    ├── README.md                          # skill-specific docs
    └── references/
        └── style-guide-template.md        # editing template the skill uses
```

## Acknowledgments

The `line-and-copy-editor` skill was inspired by and adapted from two prior projects, both used under MIT license:

**[@lfurze/claude-skills](https://github.com/lfurze/claude-skills)** — provided the docx XML editing technical reference and the multi-pass editing workflow structure.

**[@felipelobomotta-blip/book-genesis-v4](https://github.com/felipelobomotta-blip/book-genesis-v4)** — provided framing for the editor's role definition, scope boundaries, AI-prose artifact awareness, and quality-bar conventions.

Both are released under the MIT License. The required copyright notice and permission text:

```
MIT License

Copyright (c) lfurze
Copyright (c) Felipe Lobo Motta

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.
```

## License

MIT — see [LICENSE](LICENSE) for the full text. Each skill in this repo is released under the same license unless otherwise noted in the skill's own folder.

## Contributing

Issues and PRs welcome. If you have a skill you'd like to add, open an issue first to discuss whether it fits the scope of this collection.
