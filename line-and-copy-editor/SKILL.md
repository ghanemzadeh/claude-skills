---
name: line-and-copy-editor
description: >-
  Combined line and copy editing for nonfiction manuscripts: sentence-level
  prose work plus grammar, consistency, and factual cross-checks in one pass.
  Use for a line edit, copy edit, combined or stylistic edit, manuscript
  tightening or compression, SPAG and consistency work, a Chicago-style
  cleanup, removing AI-drafting and humanizer artifacts from a manuscript, or
  editing AI-assisted text toward genuinely human prose. Produces real Word
  tracked changes, a running style sheet, and an editorial cover letter.
license: MIT
allowed-tools:
  - Read
  - Write
  - Edit
  - Grep
  - Glob
  - Bash
  - AskUserQuestion
metadata:
  version: "2.1.0"
---

# Line and copy editor

This skill performs a combined line and copy edit on a nonfiction manuscript: one careful pass that does sentence-level prose work and copy editing in the same sweep. A pure copy edit fixes grammar and leaves prose rhythm alone; a pure line edit shapes prose and skips factual consistency. The combined edit covers both, on a manuscript that is structurally sound but stylistically rough.

## When to use this skill

Use when the author asks for any of:

- A "combined edit," "stylistic + copy edit," or "line and copy edit"
- A pass on a manuscript that has been through AI drafting, AI rewriting, or a "humanizer" tool and now reads unevenly
- Tightening or compression of a long-form manuscript without losing arguments
- Final polish before proofreading on a trade nonfiction book
- SPAG, consistency, and voice work in a single sweep

Do not use this skill for:

- Developmental editing (chapter restructuring, argument-level work), which is a different scope
- Pure proofreading on already-polished text, where this is too heavy a tool
- Ghostwriting or rewriting to a different voice, which the scope rules below exclude by definition

## In scope vs out of scope

**In scope:**

- Sentence-level prose: rhythm, redundancy, awkward phrasing, pacing, voice consistency across all chapters
- Compression: cut wordcount by the agreed percentage (typically 10–15%) without removing arguments; the cuts come from tightening, never from dropping points
- Grammar, spelling, punctuation
- Style consistency across chapters (em-dash spacing, quote marks, italics for titles, capitalization of defined terms)
- Factual cross-checks against what is already cited: founding dates, employee counts, valuations, name spellings of less-common figures, ship and product names
- Citation and reference alignment: in-text markers must match the reference list; bibliography entries must match what's cited

**Out of scope:**

- Rewriting voice or thesis
- Adding new arguments, examples, or sources
- Restructuring chapter order or sections
- Original fact research beyond verifying what's already cited
- Running the text through another AI rewrite pass. A manuscript that already carries machine-prose artifacts gets worse with another generation pass. Every fix in this skill is made by hand, surgically, as a tracked change the author can accept or reject.

Confirm scope explicitly with the author before starting. If they want anything in the out-of-scope list, flag it as a separate engagement.

## The no-fabrication rule

An edit may not introduce any fact, name, number, date, quote, or source that is not already in the manuscript or its citations. When a sentence needs information the manuscript does not contain (a source for a vague claim, a date behind a hedge), query the author in a comment. This rule has no exceptions; it is what separates editing nonfiction from quietly corrupting it.

## Before starting

1. Read the **Technical Reference** at the bottom of this file for docx XML editing mechanics.
2. Read `references/ai-prose-patterns.md`, the catalog of machine-drafting patterns with a default action for each. It is the core reference for the prose layer of this edit.
3. Copy `references/style-guide-template.md` and start a fresh style sheet for this manuscript.
4. Confirm with the author:
   - Style standard (default: The Chicago Manual of Style, 18th ed.)
   - Dictionary (default: Merriam-Webster at merriam-webster.com; Collegiate 11th ed. in print)
   - Variant of English (US/UK/CA/AU)
   - Em-dash convention (spaced or unspaced)
   - Oxford comma (default: yes for trade nonfiction)
   - Target wordcount or compression percentage
   - Defined terms that are capitalized as proper nouns (any coined concept the book treats as a proper noun)
   - Chunk size and delivery cadence

## AI-prose artifacts

If the manuscript has been AI-drafted or run through a humanizer tool, pattern work is the core of the edit. The full catalog lives in `references/ai-prose-patterns.md`: thirty-six patterns across six groups (content, language, style, communication, filler and rhetoric, and the mechanical debris humanizer passes leave behind), each with a default action and, where relevant, a per-chapter dose budget.

Three principles from the catalog shape everything else:

- Most patterns are bad in aggregate, not in isolation. One em dash is prose; a cluster is a tell. Look for pileups, and read the catalog's false-positives list before flagging anything.
- Sweep for mechanical artifacts (double spaces, stranded commas, quote mixing) with grep before reading for prose. They hide in clean-looking paragraphs.
- Cross-chapter consistency needs lists, not memory: recurring names, facts, defined-term capitalization. Build the lists early (see Cross-chapter consistency below) and grep against them.

## Editing toward human prose

Removing machine tells is half the prose layer. A page can be clean of every cataloged pattern and still read machine-made, because the strongest signals are document-level: how sentence lengths vary, how paragraphs are sized, how chapters end, whether insertions match the author's register. AI detectors such as Pangram are holistic classifiers trained on whole documents; scrubbing tells does not fool them, and this skill makes no attempt to. The durable edit gives the prose the qualities human writing actually has. Aim at those directly:

- **Sentence rhythm.** A human page mixes a six-word sentence with a forty-word one. Preserve that mix and restore it where drafting flattened it. When compression tightens many sentences at once, vary where the cuts land so the survivors differ in length and shape.
- **Paragraph variance.** Uniform paragraph sizes are a machine signature. Let a one-sentence paragraph stand. Never split or merge paragraphs to make the page tidier.
- **Endings.** Human conclusions run short. Cut recap padding (pattern 28) and let chapters end on their last concrete point.
- **Register.** Insertions match the author's baseline. If the author writes contractions, insertions use contractions; if the author is blunt, the insertion is blunt. Formal text spliced into a loose manuscript reads as a seam.
- **Specificity.** Human writing holds hard-to-fabricate particulars. Where the manuscript goes vague or suspiciously generic (pattern 5), the route to specificity is an author query asking for the lived detail. Never invent it.
- **Honest negativity.** Relentless positivity is a machine register. Where the author criticizes, admits uncertainty, or leaves a judgment mixed, protect it.
- **Imperfection.** A slightly awkward sentence in the author's voice beats a smooth one in nobody's. Merely imperfect is not a defect; leave it.

The catalog's "Signs of human writing" section lists what these qualities look like on the page, and the pre-delivery checklist carries the aggregate checks: rhythm variance on edited pages, register match in insertions, endings free of recap.

## Pass structure for a combined edit

A combined edit is one logical pass per chunk, but inside each chunk you are doing three things in a particular order. Doing them out of order wastes work: you'll polish a sentence at the prose layer that you then cut at the compression layer.

**Order of operations inside each chunk:**

1. **Compression and prose layer first.** Read the chunk through once. Mark sentences and paragraphs to cut, tighten, or restructure. Track-change the prose work. This is where the wordcount comes down.
2. **Copy-editing layer second.** Now that the surviving prose is settled, fix grammar, punctuation, capitalization, spelling, and style-sheet conformance.
3. **Cross-checks last.** Verify dates, names, numbers, and citations in this chunk against the running style sheet and the reference list.

Do not jump back and forth between layers within a paragraph. Finish the prose work on the chunk, then sweep for copy issues, then sweep for facts. You will catch more this way.

## Compression strategy

The wordcount target is the discipline. A 10–15% cut removes roughly one word in every seven to ten. It should come from tightening, never from removing content, and the amount of cutting in any passage should be proportional to the actual slop in it. A clean paragraph passes through untouched.

**Where the cuts come from, in priority order:**

1. Hedging phrases and meta-commentary ("It's worth noting," "As we will see," "What's interesting here").
2. Adverb pile-ups ("very," "really," "quite," "essentially," "fundamentally," "ultimately").
3. Throat-clearing sentence openers that restate what the previous paragraph already said.
4. Rule-of-three and parallel constructions where two members do the work of three.
5. Long subordinate clauses that can be promoted to their own short sentence or cut entirely.
6. Restated thesis at chapter ends. If it was clearly argued, the restatement is filler.
7. Sentences that fail the portability test: if a sentence could sit unchanged in any book on any subject, it carries no information about this one. Cut it or anchor it to something specific already in the manuscript.

**Where cuts do not come from:**

- Concrete examples, anecdotes, names, numbers, and dates. These give nonfiction its weight; compress around them.
- Author voice tics that are deliberate. If the author uses sentence fragments for rhythm, leave them and note it in the style sheet.
- Quoted material, ever.

If a passage is genuinely repetitive at the argument level (the same point made twice across chapters), don't silently cut; that is a structural call. Comment it for the author: "This argument also appears in Ch. 3, pp. X. Cut here, cut there, or keep both?"

## Track changes vs comments

The pattern catalog assigns a default action to every AI-prose pattern. Beyond those:

**Track change when:**

- The edit is concrete and unambiguous
- SPAG correction
- Style-sheet conformance fix
- Compression edit you're confident about
- Removal of AI-prose artifacts where the rebuild is clear

**Comment when:**

- The edit could go multiple ways and the author should choose
- You're querying a fact you can't verify from what's cited
- You're flagging a pattern (e.g., "third 'not just X' construction in this chapter; consider varying")
- You're noting a structural issue that's out of scope but worth raising
- You're explaining a non-obvious change

**Comment style:** terse and specific. State the issue, suggest options if useful, stop.

Good: "Date conflict: Ch. 2 says 1994, Ch. 7 implies 1995. Which?"
Bad: "I noticed that the date here doesn't match what was said earlier in the manuscript. It's important for nonfiction to be consistent on factual matters like dates, so I wanted to flag this for your attention…"

## Style sheet management

The style sheet is the most important deliverable after the manuscript itself. It documents every recurring decision and becomes the reference for any future revision or sequel.

**Start it on chunk one. Update it on every chunk.** Check it before starting each new chunk. An incomplete style sheet lets inconsistencies leak across chunks.

**Categories to track:**

- Spelling preferences (US vs UK forms; any author-specific choices)
- Capitalization rules, especially defined and coined terms used as proper nouns
- Punctuation conventions: em-dash spacing, ellipsis style, serial comma
- Number style: words vs numerals at which threshold; how percentages, money, and dates are rendered
- Italics: what gets italicized (book titles, ship names, foreign words on first use, etc.)
- Quote style: straight vs smart, single vs double for nested
- Recurring proper nouns with verified spellings, especially less-common names
- Recurring concept terms and how they're rendered
- Author voice notes: deliberate fragments, deliberate sentence-opener "And"/"But", a confirmed heavy-dash style, anything that looks like an error but is intentional. The catalog's "signs of human writing" list feeds this section; what lands here is protected from editing.

## Cross-chapter consistency

Names, dates, numbers, and concepts that recur across chapters need active tracking, not memory.

**Build three lists early (by end of chunk two or three):**

1. **Names list**: every proper noun with verified spelling. Less-common names (non-English names, less-public figures) must be checked against an authoritative source the first time they appear; subsequent appearances are checked against the names list.
2. **Facts list**: every specific date, dollar figure, employee count, valuation, and founding year, with source.
3. **Defined-terms list**: coined or capitalized concepts and how they should appear.

When editing a later chunk, grep against these lists. A discrepancy is a comment for the author, never a silent fix; the author may have meant the variant.

## Citation and reference alignment

If the manuscript has numbered citations and a reference list:

- Every in-text citation marker must point to an existing reference list entry
- Every reference list entry should have at least one in-text citation (orphans are a flag)
- Names, dates, and titles in citations must match the reference list exactly
- Format consistency across the reference list (Chicago author-date or notes-bibliography; pick one and enforce it)

Run this as its own sweep at the end of the engagement, after all chunks are edited. Verifying citations chunk by chunk costs too much context-switching.

## Calibration phase

Before editing the full manuscript, edit a sample (1,500–2,500 words, ideally one short chapter or a self-contained section) and return it to the author. Ask:

- Heaviness: too aggressive, too light, about right?
- Voice preservation: are the cuts respecting the author's tics, or smoothing them away?
- Comment density: useful, or noise?
- Compression rate on this sample: extrapolated to the full manuscript, does it hit the target?
- Any style preferences to lock into the sheet now rather than discover later?

Adjust based on feedback before continuing.

## Chunking

For manuscripts over 5,000 words:

- **Natural boundaries preferred:** chapter or major section
- **Fallback:** 3,000–5,000 words per chunk
- **Track progress:** mark which chunks are done; note running wordcount delta against target

Per chunk:

1. Unpack docx to XML (Technical Reference below)
2. Read once for prose and compression
3. Track-change prose work
4. Sweep for copy issues
5. Sweep for facts and style-sheet conformance
6. Pack back to docx
7. Run `references/pre-delivery-checklist.md`; fix anything that fails before delivering
8. Update style sheet, names list, facts list
9. Move to next chunk

## Quality bar

When the engagement is done:

- Final wordcount within the agreed target band
- A test reader who hasn't seen the source cannot reliably tell which sentences were AI-drafted and which were human-drafted
- Zero factual contradictions across chapters for any specific date, number, or name
- Zero discrepancies between in-text citations and the reference list
- Style sheet complete enough that someone else could pick up a future revision and stay consistent
- Rhythm intact at page scale: sentence and paragraph lengths in edited pages vary at least as much as in the author's cleanest untouched ones
- Author voice intact. This is the criterion that fails most often: if the author reads the edited version and feels smoothed into someone else, the edit is too heavy, however clean the prose reads.

## Deliverables

1. **Edited manuscript with tracked changes**, one Word file per chapter (or one combined file, depending on author preference). All edits as track changes; queries as comments.
2. **Editorial cover letter**: overall read of the book, voice and tone observations, structural issues noticed but not fixed (structure is out of scope), inconsistencies you couldn't resolve, anything the author should know before proofread.
3. **Style sheet**: every choice documented, organized by the categories above.
4. **Names list and facts list**, appended to the style sheet or delivered separately.
5. **Second-pass cleanup** on issues the first pass introduced (typos in inserted text, broken citation numbering after compression, etc.), included in the engagement.

## Default style standards

If the author hasn't specified, default to:

- The Chicago Manual of Style, 18th edition (2024)
- Merriam-Webster at merriam-webster.com (Collegiate Dictionary, 11th ed., in print)
- American English
- Smart (curly) quotes
- Em-dashes unspaced (no space before or after)
- Oxford comma: yes
- Numbers: spell out under 100 in narrative prose; figures for percentages, money, dates, and valuations regardless of size
- Italics: book titles, film titles, ship and aircraft names, foreign words on first use only
- Defined and coined terms capitalized as proper nouns where the author has signaled this; document in the style sheet on first encounter

Note one deliberate divergence from web-oriented de-slopping tools such as humanizer: those ban em dashes and curly quotes outright, because on the web they read as machine tells. In book publishing both are standard. This skill keeps them and polices density instead; the calibrated em-dash rule is pattern 14 in `references/ai-prose-patterns.md`.

Confirm any deviations with the author and lock them into the style sheet at the top.

---

## Technical Reference: Docx XML Editing

Word `.docx` files are ZIP archives containing XML. To produce real Word track changes that the author can accept or reject in Review mode, edit the XML directly.

### Unpack

```bash
mkdir -p work
cp manuscript.docx work/original-backup.docx
unzip -o manuscript.docx -d work/manuscript_xml
```

The body lives in `work/manuscript_xml/word/document.xml`.

### Allocate revision IDs first

Every `w:id` on `w:ins`, `w:del`, and comment elements must be unique across the document. Before the first edit, find the highest existing ID:

```bash
grep -ohE 'w:id="[0-9]+"' work/manuscript_xml/word/document.xml \
  work/manuscript_xml/word/comments.xml \
  work/manuscript_xml/word/footnotes.xml \
  work/manuscript_xml/word/endnotes.xml 2>/dev/null \
  | grep -oE '[0-9]+' | sort -n | tail -1
```

Start your counter above that number and keep one running counter across all chunks. Record the high-water mark in your working notes so the next chunk doesn't collide.

### Insertions

```xml
<w:ins w:id="101" w:author="Editor" w:date="2026-01-15T10:00:00Z">
  <w:r>
    <w:t xml:space="preserve">inserted text </w:t>
  </w:r>
</w:ins>
```

### Deletions

```xml
<w:del w:id="102" w:author="Editor" w:date="2026-01-15T10:00:00Z">
  <w:r>
    <w:delText xml:space="preserve">deleted text </w:delText>
  </w:r>
</w:del>
```

### Replacements

A `<w:del>` immediately followed by a `<w:ins>` at the same location.

### Deleting a whole paragraph

Compression edits often cut entire paragraphs, and wrapping the runs in `<w:del>` is not enough: the paragraph mark survives, and accepting the change leaves an empty paragraph behind. Mark the pilcrow deleted as well, inside the paragraph properties:

```xml
<w:p>
  <w:pPr>
    <w:rPr>
      <w:del w:id="103" w:author="Editor" w:date="2026-01-15T10:00:00Z"/>
    </w:rPr>
  </w:pPr>
  <w:del w:id="104" w:author="Editor" w:date="2026-01-15T10:00:00Z">
    <w:r>
      <w:delText xml:space="preserve">The whole paragraph being cut.</w:delText>
    </w:r>
  </w:del>
</w:p>
```

On accept, the paragraph merges into the following one and disappears cleanly.

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
<w:comment w:id="10" w:author="Editor" w:date="2026-01-15T10:00:00Z" w:initials="Ed">
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

**Modern comment parts.** Documents saved by recent Word versions may also carry `word/commentsExtended.xml` and `word/commentsIds.xml` (threading and resolution metadata keyed by paragraph `paraId`). When they exist, leave them in place; deleting them can make Word drop or mis-thread comments. When they don't exist, plain `comments.xml` plus the relationship and content-type entries above is sufficient.

### Repack

```bash
(cd work/manuscript_xml && zip -r -X ../../manuscript_edited.docx . -x ".*")
```

The `-X` flag strips macOS extended attributes, and the subshell keeps your working directory unchanged. `[Content_Types].xml` must sit at the archive root, which it will if you zip from inside `manuscript_xml`.

### Validate after every repack

```bash
unzip -t manuscript_edited.docx
xmllint --noout work/manuscript_xml/word/document.xml
xmllint --noout work/manuscript_xml/word/comments.xml 2>/dev/null
grep -ohE '<w:(ins|del|comment) [^>]*w:id="[0-9]+"' work/manuscript_xml/word/document.xml \
  | grep -oE 'w:id="[0-9]+"' | sort | uniq -d
```

The last command must print nothing (no duplicate revision IDs). Then open the file in Word or LibreOffice and confirm the changes appear in the Review pane and can be accepted or rejected one at a time.

### Tips

- Back up the original before editing (the unpack step above does this).
- Preserve all existing XML attributes and namespaces; touch text content, not structure.
- Watch `xml:space="preserve"` on `<w:t>` and `<w:delText>`. It controls whitespace and is easy to break.
- For markdown source converted to docx (pandoc, etc.), expect simpler XML: fewer `rsid` attributes, cleaner runs. Track changes work the same way.
