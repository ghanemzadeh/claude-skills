---
name: line-and-copy-editor
description: "Combined line editing and copy editing for nonfiction manuscripts in a single sweep — sentence-level prose work plus grammar, consistency, and factual cross-checks. Especially suited to manuscripts that have been through AI-assisted drafting or 'humanizer' passes and now need one careful pass to remove machine-prose artifacts, tighten rhythm, and lock down style. Produces tracked-changes Word output, a running style sheet, and an editorial cover letter. MANDATORY TRIGGERS: combined edit, line edit, copy edit, stylistic edit, line and copy edit, tighten manuscript, compress manuscript, remove AI artifacts, dehumanize / humanize cleanup, SPAG + style, Chicago style edit"
---

# Line and Copy Editor

A combined line + copy edit on a nonfiction manuscript. One careful pass that does sentence-level prose work *and* copy-editing in the same sweep — not two separate engagements, not a developmental edit, not a bare proofread.

The split matters. Pure copy editors fix grammar and miss prose rhythm. Pure line editors fix prose and skip factual consistency. This skill does both, in one pass, on a manuscript that is structurally sound but stylistically rough.

## When to use this skill

Use when the author asks for any of:

- A "combined edit," "stylistic + copy edit," or "line and copy edit"
- A pass on a manuscript that has been through AI drafting, AI rewriting, or a "humanizer" tool and now reads unevenly
- Tightening / compression of a long-form manuscript without losing arguments
- Final polish before proofreading on a trade nonfiction book
- SPAG + consistency + voice in a single sweep

Do **not** use this skill for:

- Developmental editing (chapter restructuring, argument-level work) — that is a different scope
- Pure proofreading on already-polished text — too heavy a tool
- Ghostwriting or rewriting to a different voice — out of scope by definition

## In scope vs out of scope

**In scope:**

- Sentence-level prose: rhythm, redundancy, awkward phrasing, pacing, voice consistency across all chapters
- Compression: cut wordcount by the agreed percentage (typically 10–15%) without removing arguments — tighten, don't trim points
- Grammar, spelling, punctuation
- Style consistency across chapters (em-dash spacing, quote marks, italics for titles, capitalization of defined terms)
- Factual cross-checks against what is already cited: founding dates, employee counts, valuations, name spellings of less-common figures, ship/product names
- Citation/reference alignment: in-text markers must match the reference list; bibliography entries must match what's cited

**Out of scope:**

- Rewriting voice or thesis
- Adding new arguments, examples, or sources
- Restructuring chapter order or sections
- Original fact research beyond verifying what's already cited
- Running the text through another AI rewrite pass — if the manuscript already has machine-prose artifacts, another generation pass compounds the problem rather than fixing it. Edit by hand, surgically.

Confirm scope explicitly with the author before starting. If they want anything in the "out of scope" list, flag it as a separate engagement.

## Before starting

1. Read the **Technical Reference** at the bottom of this file for docx XML editing mechanics.
2. Read `references/style-guide-template.md` (if present) and start a fresh style sheet for this manuscript.
3. Confirm with the author:
   - Style standard (default: Chicago Manual of Style, 17th ed.)
   - Dictionary (default: Merriam-Webster's Collegiate, 11th ed.)
   - Variant of English (US/UK/CA/AU)
   - Em-dash convention (spaced or unspaced)
   - Oxford comma (default: yes for trade nonfiction)
   - Target wordcount or compression percentage
   - Defined terms that are capitalized as proper nouns (any coined concept the book treats as a proper noun)
   - Chunk size and delivery cadence

## AI-prose artifacts to watch for

This is the most important section if the manuscript has been AI-drafted or run through a humanizer. These patterns are not "bad writing" in isolation — they are bad in *aggregate*, because they signal machine drafting. Editing them out is the core of what makes the manuscript pass as human-written.

**Mechanical artifacts from humanizer passes:**

- Stranded commas where em-dashes were converted (",, " sequences, comma-then-space-then-capital where a dash was)
- Em-dash → comma swaps that break sentence rhythm
- Double spaces between sentences
- Broken bulleted or numbered lists (orphaned markers, inconsistent indentation)
- Smart-quote / straight-quote mixing within the same paragraph

**Repetitive prose patterns:**

- Rhetorical inversions overused: "This was not just X. It was Y." Allow one or two per chapter; flag the third.
- Triadic structures: chains of three parallel noun phrases ("the X, the Y, the Z") — flag when they recur within a few pages.
- Hedging openers: "It is worth noting that," "What's interesting is," "Importantly," "Notably" — almost always cuttable.
- Sentence-opener "And" / "But" used to manufacture rhythm. Some are fine; flag clusters.
- "Not just X — Y" constructions stacked back to back.
- Em-dash dependency: any sentence with **three or more em-dashes** is a flag — read it aloud and rebuild.

**Cross-chapter inconsistencies:**

- Recurring people, places, and concepts must be referred to identically. Build a names list early and grep across chapters.
- The same fact stated two ways (e.g., "founded in 1994" in Ch. 2, "founded the year before Amazon launched its bookstore" in Ch. 7 — pick one and make sure both parse correctly).
- Drift in defined-term usage. A coined concept that the manuscript capitalizes as a proper noun must stay capitalized everywhere; a single lowercase appearance is a slip, not a stylistic choice.

## Pass structure for a combined edit

A combined edit is one logical pass per chunk, but inside each chunk you are doing three things in a particular order. Doing them out of order wastes work — you'll polish a sentence at the prose layer that you then cut at the compression layer.

**Order of operations inside each chunk:**

1. **Compression and prose layer first.** Read the chunk through once. Mark sentences and paragraphs to cut, tighten, or restructure. Track-change the prose work. This is where the wordcount comes down.
2. **Copy-editing layer second.** Now that the surviving prose is settled, fix grammar, punctuation, capitalization, spelling, and style-sheet conformance.
3. **Cross-checks last.** Verify dates, names, numbers, and citations in this chunk against the running style sheet and the reference list.

Do not jump back and forth between layers within a paragraph. Finish the prose work on the chunk, then sweep for copy issues, then sweep for facts. You will catch more this way.

## Compression strategy

The wordcount target is the discipline. If you're asked to cut 10–15%, that's roughly one word in every seven or eight — meaningful, but it should come from tightening, not from removing content.

**Where the cuts come from, in priority order:**

1. Hedging phrases and meta-commentary ("It's worth noting," "As we will see," "What's interesting here").
2. Adverb pile-ups ("very," "really," "quite," "essentially," "fundamentally," "ultimately").
3. Throat-clearing sentence openers that restate what the previous paragraph already said.
4. Triadic and parallel constructions where two members do the work of three.
5. Long subordinate clauses that can be promoted to their own short sentence or cut entirely.
6. Restated thesis at chapter ends — if it was clearly argued, the restatement is filler.

**Where cuts do *not* come from:**

- Concrete examples, anecdotes, names, numbers, dates — these are the ballast of nonfiction. Compress around them, not through them.
- Author voice tics that are deliberate. If the author uses sentence fragments for rhythm, leave them. Note in the style sheet.
- Quoted material.

If a passage is genuinely repetitive at the argument level (the same point made twice across chapters), don't silently cut — that's structural. Comment it for the author: "This argument also appears in Ch. 3, pp. X. Cut here, cut there, or keep both?"

## Track changes vs comments

**Track change when:**

- The edit is concrete and unambiguous
- SPAG correction
- Style-sheet conformance fix
- Compression edit you're confident about
- Removal of AI-prose artifacts where the rebuild is clear

**Comment when:**

- The edit could go multiple ways and the author should choose
- You're querying a fact you can't verify from what's cited
- You're flagging a pattern (e.g., "third 'not just X — Y' construction in this chapter; consider varying")
- You're noting a structural issue that's out of scope but worth raising
- You're explaining a non-obvious change

**Comment style:** terse and specific. State the issue, suggest options if useful, stop.

Good: "Date conflict — Ch. 2 says 1994, Ch. 7 implies 1995. Which?"
Bad: "I noticed that the date here doesn't match what was said earlier in the manuscript. It's important for nonfiction to be consistent on factual matters like dates, so I wanted to flag this for your attention…"

## Style sheet management

The style sheet is the single most important deliverable after the manuscript itself. It documents every recurring decision and becomes the reference for any future revision or sequel.

**Start it on chunk one. Update it on every chunk.** Check it before starting each new chunk.

**Categories to track:**

- Spelling preferences (US vs UK forms; any author-specific choices)
- Capitalization rules — especially defined/coined terms used as proper nouns
- Punctuation conventions — em-dash spacing, ellipsis style, serial comma
- Number style — words vs numerals at which threshold; how percentages, money, dates are rendered
- Italics — what gets italicized (book titles, ship names, foreign words on first use, etc.)
- Quote style — straight vs smart, single vs double for nested
- Recurring proper nouns with verified spellings, especially less-common names
- Recurring concept terms and how they're rendered
- Author voice notes — deliberate fragments, deliberate sentence-opener "And"/"But", anything that *looks* like an error but is intentional

A complete style sheet is the sign of a real combined edit. An incomplete one means inconsistencies will leak across chunks.

## Cross-chapter consistency

Names, dates, numbers, and concepts that recur across chapters need active tracking, not memory.

**Build three lists early (by end of chunk two or three):**

1. **Names list** — every proper noun with verified spelling. Less-common names (non-English names, less-public figures) must be checked against an authoritative source the *first* time they appear; subsequent appearances are checked against the names list.
2. **Facts list** — every specific date, dollar figure, employee count, valuation, founding year. With source.
3. **Defined-terms list** — coined or capitalized concepts and how they should appear.

When editing a later chunk, grep against these lists. A discrepancy is a comment for the author, not a silent fix — the author may have meant the variant.

## Citation and reference alignment

If the manuscript has numbered citations and a reference list:

- Every in-text citation marker must point to an existing reference list entry
- Every reference list entry should have at least one in-text citation (orphans are a flag)
- Names, dates, and titles in citations must match the reference list exactly
- Format consistency across the reference list (Chicago author-date or notes-bibliography — pick one and enforce)

This is its own sweep at the end of the engagement, after all chunks are edited. Do not try to verify citations chunk by chunk — too much context-switching.

## Calibration phase

Before editing the full manuscript, edit a sample (1,500–2,500 words, ideally one short chapter or a self-contained section) and return it to the author. Ask:

- Heaviness: too aggressive, too light, about right?
- Voice preservation: are the cuts respecting the author's tics, or smoothing them away?
- Comment density: useful, or noise?
- Compression rate on this sample — extrapolated to the full manuscript, does it hit the target?
- Any style preferences to lock into the sheet now rather than discover later?

Adjust based on feedback before continuing. This 30-minute step prevents days of rework.

## Chunking

For manuscripts over 5,000 words:

- **Natural boundaries preferred:** chapter or major section
- **Fallback:** 3,000–5,000 words per chunk
- **Track progress:** mark which chunks are done; note running wordcount delta against target

Per chunk:

1. Unpack docx → XML (Technical Reference below)
2. Read once for prose / compression
3. Track-change prose work
4. Sweep for copy issues
5. Sweep for facts and style-sheet conformance
6. Pack back to docx
7. Update style sheet, names list, facts list
8. Move to next chunk

## Quality bar

When the engagement is done:

- Final wordcount within the agreed target band
- A test reader who hasn't seen the source cannot reliably tell which sentences were AI-drafted vs. human-drafted
- Zero factual contradictions across chapters for any specific date, number, or name
- Zero discrepancies between in-text citations and the reference list
- Style sheet is complete enough that someone else could pick up a future revision and stay consistent
- Author voice is intact — the manuscript still sounds like the author, not the editor

The voice test is the one that's easy to fail. If the author reads the edited version and feels they've been smoothed into someone else, the edit is too heavy regardless of how clean the prose reads.

## Deliverables

1. **Edited manuscript with tracked changes**, one Word file per chapter (or one combined file, depending on author preference). All edits as track changes; queries as comments.
2. **Editorial cover letter** — overall read of the book: voice/tone observations, structural issues noticed but not fixed (since structure is out of scope), inconsistencies you couldn't resolve, anything the author should know before proofread.
3. **Style sheet** — every choice documented, organized by the categories above. This is the reference doc for any future revision.
4. **Names list and facts list** — appended to the style sheet or delivered separately.
5. **Second-pass cleanup** on issues the first pass introduced (typos in inserted text, broken citation numbering after compression, etc.) — included in the engagement, not a separate fee.

## Default style standards

If the author hasn't specified, default to:

- Chicago Manual of Style, 17th edition
- Merriam-Webster's Collegiate Dictionary, 11th edition
- American English
- Smart (curly) quotes
- Em-dashes unspaced (no space before or after)
- Oxford comma: yes
- Numbers: spell out under 100 in narrative prose; figures for percentages, money, dates, and valuations regardless of size
- Italics: book titles, film titles, ship/aircraft names, foreign words on first use only
- Defined/coined terms capitalized as proper nouns where the author has signaled this; document in the style sheet on first encounter

Confirm any deviations with the author and lock them into the style sheet at the top.

---

## Technical Reference: Docx XML Editing

Word `.docx` files are ZIP archives containing XML. To produce real Word track changes that the author can accept/reject in Review mode, edit the XML directly.

### Unpack

```bash
mkdir -p work && cp manuscript.docx work/manuscript.zip && cd work && unzip manuscript.zip -d manuscript_xml
```

The body lives in `manuscript_xml/word/document.xml`.

### Insertions

```xml
<w:ins w:id="1" w:author="Editor" w:date="2025-01-15T10:00:00Z">
  <w:r>
    <w:t xml:space="preserve">inserted text </w:t>
  </w:r>
</w:ins>
```

### Deletions

```xml
<w:del w:id="2" w:author="Editor" w:date="2025-01-15T10:00:00Z">
  <w:r>
    <w:delText xml:space="preserve">deleted text </w:delText>
  </w:r>
</w:del>
```

### Replacements

A `<w:del>` immediately followed by a `<w:ins>` at the same location.

### Comments

Two places in the docx:

**1. Markers in `document.xml`:**

```xml
<w:commentRangeStart w:id="10"/>
<!-- the commented runs -->
<w:commentRangeEnd w:id="10"/>
<w:r>
  <w:rPr><w:rStyle w:val="CommentReference"/></w:rPr>
  <w:commentReference w:id="10"/>
</w:r>
```

**2. Content in `word/comments.xml`:**

```xml
<w:comment w:id="10" w:author="Editor" w:date="2025-01-15T10:00:00Z" w:initials="Ed">
  <w:p><w:r><w:t>Comment text.</w:t></w:r></w:p>
</w:comment>
```

If `comments.xml` doesn't exist, create it with proper namespace declarations and add:

In `word/_rels/document.xml.rels`:
```xml
<Relationship Id="rIdComments" Type="http://schemas.openxmlformats.org/officeDocument/2006/relationships/comments" Target="comments.xml"/>
```

In `[Content_Types].xml`:
```xml
<Override PartName="/word/comments.xml" ContentType="application/vnd.openxmlformats-officedocument.wordprocessingml.comments+xml"/>
```

### Repack

```bash
cd manuscript_xml && zip -r ../manuscript_edited.docx . -x ".*" && cd ..
```

### Tips

- Every `w:id` (for `w:ins`, `w:del`, comments) must be unique across the document. Use incrementing integers.
- Back up the original before editing.
- Validate by opening in Word or LibreOffice after each chunk.
- Preserve all existing XML attributes and namespaces — touch text content, not structure.
- Watch `xml:space="preserve"` on `<w:t>` and `<w:delText>` — it controls whitespace and is easy to break.
- For markdown source converted to docx (pandoc, etc.), expect simpler XML — fewer `rsid` attributes, cleaner runs. Track changes still work the same way.
