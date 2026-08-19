# AI-prose pattern catalog

Read this file before editing the first chunk. It lists the patterns that mark a manuscript as machine-drafted, what each looks like, and what an editor does about each one inside a track-changes workflow.

Two rules govern every entry:

1. **This is surgery, not regeneration.** Fix each instance with the smallest edit that works. Never rewrite a passage wholesale and never run text through another generation pass.
2. **Never fabricate.** An edit may not introduce any fact, name, number, date, quote, or source that is not already in the manuscript or its citations. When a sentence needs information the manuscript does not contain (a source for a vague claim, a date for a hedge), the correct move is a query comment to the author.

## How to read an entry

- **Watch for** lists trigger words or shapes. All quoted material in this file is an example of the problem, kept for recognition. Do not flag this file's own examples.
- **Default action** is one of:
  - *Track change*: the fix is unambiguous; make it.
  - *Comment*: judgment call, missing information, or a pattern worth the author's attention; query, do not silently fix.
  - *Cover letter*: structural, out of scope for the edit itself; note it in the editorial cover letter.
  - *Leave*: within dose, or a legitimate stylistic choice.
- **Dose** appears where a pattern is only a problem in aggregate. Track tallies per chapter in your working notes. One instance of most of these patterns is ordinary writing; the tell is density.

## Group 1: Content patterns

### 1. Significance inflation

Watch for: "marks a pivotal moment", "stands as a testament", "underscores the importance", "reflects broader trends", "setting the stage for", "indelible mark", "key turning point", "evolving landscape".

Statements that puff up an event or detail by tying it to sweeping importance. The sentence usually survives with the inflation cut.

Default action: Track change. Delete the inflating clause; keep the factual core.
Fix: "The institute was established in 1989, marking a pivotal moment in regional statistics" becomes "The institute was established in 1989."

### 2. Notability padding

Watch for: lists of media outlets with no context ("has been cited in the Times, the BBC, and the Financial Times"), follower counts, "written by a leading expert".

Default action: Track change if one citation in the list carries real context in the manuscript (keep that one, cut the roll call). Comment if none do: ask the author which mention matters and what was actually said. Do not invent the context.
Dose: a single contextualized citation is fine; the roll call is the tell.

### 3. Superficial "-ing" analysis

Watch for: trailing participle clauses that pretend to explain: "…, highlighting", "…, reflecting", "…, symbolizing", "…, showcasing", "…, ensuring", "…, fostering", "…, emphasizing", "…, underscoring", "…, encompassing".

The clause asserts meaning the sentence has not earned. Cutting it almost never loses information.

Default action: Track change. Delete the clause, or promote it to its own sentence if the manuscript elsewhere supports the claim.
Fix: "The palette uses blue and gold, reflecting the community's deep connection to the land" becomes "The palette uses blue and gold." If the connection is real and sourced in the manuscript, state it as its own sourced sentence.

### 4. Promotional language

Watch for: "vibrant", "nestled", "breathtaking", "renowned", "stunning", "rich cultural heritage", "boasts", "in the heart of", "must-visit", "groundbreaking" (figurative), "commitment to excellence".

Ad copy in the middle of nonfiction. The neutral version is nearly always shorter.

Default action: Track change to the neutral statement.
Fix: "Nestled in the breathtaking region of Gonder, the town boasts a rich heritage" becomes "The town is in the Gonder region."

### 5. Vague attribution and generic specifics

Watch for: "experts argue", "observers have noted", "industry reports suggest", "studies show", "critics say", "it is widely believed", with no named source.

Watch for, second form: detail that gestures at specificity without containing any. Anecdote characters with a first name and a job title only ("Sarah, a marketing manager"), "a mid-sized company in the Midwest", suspiciously round numbers with no source, an example that would fit any book on the subject unchanged. Generated anecdotes cluster on the same stock names and settings; a real person comes with a surname, a place, a year, or an odd particular.

Both forms need information only the author has, so this is the pattern an editor must never fix directly.

Default action: Comment, always. For attribution: "Which experts? Needs a named source or a cut." For a generic specific: "Is this a real person or company? If real, an anchoring detail (full name, place, year) would carry it. If illustrative or composite, say so in the text." If the manuscript cites a real source nearby, a track change attaching the claim to that source is allowed. The specificity must come from the author; never invent it.
Dose: none. Every unsourced attribution and every generic specific gets flagged.

### 6. Formulaic sections

Watch for: "Challenges and Future Prospects", "Despite these challenges…", "Future Outlook", "Conclusion" sections that restate the chapter, any section whose structure could be pasted into a different book unchanged.

Default action: Comment on the section plus a cover-letter note. Restructuring is out of scope, but the author should know the section reads as boilerplate.

## Group 2: Language patterns

### 7. AI vocabulary

Watch for, tier one (near-certain tells, cut or replace on sight): delve, tapestry (abstract), landscape (abstract), interplay, testament, underscore (verb), showcase (verb), foster, garner, gate/gated/gating (figurative; established technical senses such as feature gating stay), elevate, embark, harness, supercharge, leverage (verb), utilize, facilitate, empower, streamline, paradigm shift, game changer, transformative, cutting-edge, robust (figurative).

Watch for, tier two (fine alone, a tell in clusters): crucial, pivotal, key (adjective), vital, enduring, intricate, vibrant, enhance, highlight (verb), valuable, notably, additionally, moreover, align with, emphasize, quietly (as drama: "quietly became").

Default action: Track change to the plain word ("use" for "utilize", "build" for "foster", "run through" for "delve into"). Tier two: leave singles, thin clusters. Empty adverbs ("actually", "literally", "simply") live in pattern 21.
Dose: tier one, zero tolerance. Tier two, flag when three or more land in a paragraph.

### 8. Copula avoidance

Watch for: "serves as", "stands as", "functions as", "represents" (for "is"), "boasts", "features", "offers" (for "has").

Default action: Track change to "is", "are", "has".
Fix: "The gallery serves as the exhibition space and boasts four rooms" becomes "The gallery is the exhibition space and has four rooms."

### 9. Negative parallelism and binary contrast

Watch for: "It's not just X. It's Y.", "not only… but also", "This isn't about X, it's about Y", negative listing ("not X, not Y, but Z"), tailing negation fragments ("no guessing", "no wasted motion").

The information is in Y. State Y.

Default action: Track change within dose logic below.
Dose: allow one or two clean instances per chapter where the contrast genuinely earns its place; track-change the rest and leave a comment on the chapter's pattern once ("third 'not just X' in this chapter; I've rebuilt two, flagging the shape for your eye").

### 10. Rule of three

Watch for: chains of three parallel items where two would do or where the third is padding ("innovation, inspiration, and industry insights"), triple noun-phrase appositions ("the X, the Y, the Z").

Genuine triads exist; the tell is recurrence and padding.

Default action: Track change when a member is clearly filler (cut to two, or to the one that matters). Leave real triads.
Dose: flag when triads recur within a few pages.

### 11. Synonym cycling and repeated sentence openings

Watch for: the same referent renamed each mention ("the protagonist… the main character… the central figure… the hero"); consecutive sentences opening on the same subject and shape ("She noted the door. She noted the lock on it. She filed both away.").

Cycling fakes variety the prose does not need; repeated openings drop variety it does. Both come from handling repetition by rule instead of by ear.

Default action: Track change. For cycling, repeat the right word; repetition of a precise term is correct style. For repeated openings, merge the sentences, change one subject, or open one on the action. Fix the shape, not the repeated word; the surviving sentence may still start with "She". Deliberate repetition that builds pressure ("She came. She saw. She conquered.") is voice. For rhythm problems at passage scale, see pattern 27.

### 12. False ranges

Watch for: "from X to Y" where X and Y sit on no meaningful scale ("from the singularity of the Big Bang to the enigmatic dance of dark matter").

Default action: Track change to a plain list of what is actually covered.

### 13. Passive voice and subjectless fragments

Watch for: actorless constructions ("mistakes were made", "the decision was reached"), verbless fragments doing a sentence's job ("No configuration needed.").

Passive voice is legitimate when the actor is unknown or beside the point. The tell is passives that hide an actor the sentence needs, and fragment stacks.

Default action: Track change when the active version is clearer and the actor is in the manuscript. Leave justified passives.

## Group 3: Style patterns

Where this catalog diverges from humanizer: humanizer edits web prose and bans em dashes and curly quotes outright. This skill edits book manuscripts to publishing standards, where both are legitimate. The rules below are calibrated for that context; they treat density, not existence, as the tell.

### 14. Em-dash density

Watch for: more than one em dash per paragraph, dashes appearing in consecutive paragraphs, any sentence carrying two or more.

Chicago permits em dashes and this skill's default style keeps them, unspaced. Density is still among the strongest machine-drafting tells.

Default action: Track change any sentence with two or more em dashes (read aloud, rebuild with commas, a colon, parentheses, or a sentence break). For paragraph-level clusters, track-change the weakest dashes and add one comment noting the pattern. Record the author's deliberate dash style on the style sheet; a confirmed heavy-dash voice overrides this rule, per the style sheet.
Dose: a lone em dash used well is good prose. Leave it.

### 15. Quotation mark policy

Watch for: straight quotes in a manuscript that should ship with smart quotes; apostrophes rendered as straight ticks.

Book publishing uses smart (curly) quotes. Here they are a requirement, never a tell. Mixing is the artifact; see pattern 36 for the mechanical sweep.

Default action: Track change straight to smart, per the style sheet.

### 16. Decorative emphasis

Watch for: mechanical boldface on key terms, bullet lists whose items open with a bolded header and a colon, emoji in headings or lists, bullets carrying what should be a prose paragraph.

Rare in trade nonfiction, common in AI-drafted chapters that began life as an outline.

Default action: Comment first (formatting can be a design decision the author or publisher owns); track change when the author has already confirmed prose conventions on the style sheet.

### 17. Heading conventions

Watch for: title case where the book's convention is sentence case (or drift between the two), a heading followed by a one-line warm-up that restates the heading before the content starts.

Default action: Track change case drift to the style-sheet convention. Track-change delete restater lines; the section should open with its first real sentence.

## Group 4: Communication patterns

Chat residue: text written to a user that survived into the manuscript. All of it is a track-change deletion.

### 18. Chatbot artifacts

Watch for: "I hope this helps", "Let me know if", "Would you like me to", "Certainly!", "Here is an overview of", "In this section, we will".

Default action: Track change, delete. If deletion leaves a hole, open the section on its first substantive sentence.

### 19. Knowledge-cutoff disclaimers and speculative gap-filling

Watch for: "as of this writing" (when nothing dates it), "while specific details are scarce", "based on available information", "maintains a low profile", "likely grew up", "it is believed that".

Two forms: the disclaimer that narrates a research gap, and the invented filler that papers over one. Both are dangerous in nonfiction because the filler reads as fact.

Default action: Track change deletes the disclaimer framing. The underlying gap gets a comment: "Source for this? As written it's a guess dressed as fact." Never fill the gap yourself.

### 20. Sycophantic register

Watch for: "Great question", "You're absolutely right", reader-flattering asides ("as the savvy reader will have noticed").

Default action: Track change, delete.

## Group 5: Filler, hedging, and rhetoric

### 21. Filler phrases and empty adverbs

Watch for: "in order to", "due to the fact that", "at this point in time", "it is important to note that", "it's worth noting", "when it comes to", "at the end of the day", "in today's world", "going forward"; adverbs doing no work: "very", "really", "quite", "actually", "literally", "simply", "truly", "essentially", "fundamentally", "ultimately".

Default action: Track change. These are the first cuts in any compression pass.

### 22. Hedge stacking

Watch for: multiple qualifiers on one claim ("could potentially possibly be argued that… might"); caveat tics accumulating across a passage: "to be fair", "it's also possible", "might arguably", "in some cases it may".

One hedge is honesty; a stack is evasion. Revision loops add qualifiers a pass at a time until every claim sounds unsure. Keep the strongest single qualifier the claim deserves, and cut caveats that exist only to repair an earlier overstatement.

Default action: Track change to one hedge or none.

### 23. Throat-clearing and signposting

Watch for: "Let's dive in", "let's explore", "let's break this down", "now let's look at", "here's what you need to know", "without further ado", "heads up", "quick note", "before I forget"; conversational hooks used as fake-candid openers ("Honestly?", "Look,", "Here's the thing", "Let's be honest"); rhetorical setups ("What if I told you", "Think about it").

The announcement can wear a casual register too ("one thing that bit me hard, so pay attention to this part:"). Remove the announcement, not just its formal tone.

Default action: Track change, delete; the paragraph starts at its first real claim. Leave "honestly" and "look" when they occur mid-sentence in a genuinely conversational voice; the tell is the standalone theatrical opener.

### 24. Authority tropes, faux-insight setups, and significance narration

Watch for: "the real question is", "at its core", "what really matters", "the deeper issue", "the heart of the matter"; "what most people miss", "what nobody tells you", "the part everyone gets wrong"; and, after a point has been made, commentary narrating its weight: "That last part matters more than it sounds", "This distinction matters", "The key point is", "As you can see", "Read that again", a redundant "In other words".

The setup puts ceremony before the point; the narration puts ceremony after it. Either way the sentence tells the reader the point matters instead of making it matter.

Default action: Track change. Keep the point, cut the ceremony. When the point does not read clearly without the aside, the fix belongs in the point's own sentence, built from support already in the manuscript.

### 25. Colon reveals

Watch for: a dramatic pause-and-reveal built on a colon ("The answer: nobody knows.", "One word: leverage.").

Default action: Track change into a plain sentence when the reveal adds no information. Leave a colon doing honest work (introducing a list, an explanation, a quotation).
Dose: one per chapter can be voice. A recurring cadence is a tell.

### 26. Aphorism formulas and fake-profound kickers

Watch for: "X is the Y of Z", "X is not a tool but a mirror", "the currency of", "the architecture of"; closing lines that reach for quotability ("In the end, the market wasn't buying software. It was buying belief.").

Default action: Track change. Replace the formula with the concrete claim it gestures at. Delete kickers outright and end on the last concrete point; do not rewrite a fake-profound line into a better metaphor.

### 27. Manufactured staccato and robotic rhythm

Watch for: runs of clipped fragments engineered for drama ("No aesthetic prior. No nostalgia. The old rules were gone."); paragraphs where every sentence has the same length and shape; every paragraph landing on a punchline; pages where sentence length barely varies; chapters whose paragraphs all run to the same size.

One short sentence for emphasis is human writing. A run of them is percussion. Uniformity is the same tell at document scale: a human page mixes a six-word sentence with a forty-word one, and a two-line paragraph with a half-page one, where generated pages average out. On a suspect page, count words per sentence (the pre-delivery checklist has a spot check); when most sentences land within a few words of the mean, read the page aloud before deciding anything.

Default action: Comment, usually. Rhythm rebuilds are voice-level judgment calls; propose the rebuild in a comment during calibration, then apply the agreed treatment as track changes in later chunks. Track change directly only when the fix is a simple merge of two fragments. For document-level monotony, comment during calibration and propose where the variance should come from: splitting one overlong sentence, merging two clipped ones, letting a short paragraph stand alone. Variance comes from cuts and merges of what is already there, never from padding.

### 28. Generic conclusions and recap endings

Watch for: "The future looks bright", "Exciting times lie ahead", "a major step in the right direction"; final paragraphs opening "In conclusion", "In summary", or "Overall"; chapter endings that summarize the chapter just read, sized like a term paper's.

Human conclusions run short; a chapter that has made its argument can simply stop.

Default action: Track change. Cut the send-off; end on the last concrete fact, takeaway, or forward action the manuscript actually supports. A recap that the author clearly built as a pedagogical device gets a comment instead.

### 29. Hyphenation drift in compound pairs

Watch for: compounds hyphenated in predicate position ("the report is high-quality", "the team is cross-functional").

Hyphenate attributive use ("a high-quality report"); drop the hyphen after the noun ("the report is high quality"). Uniform hyphenation everywhere is a machine habit.

Default action: Track change; record the convention on the style sheet.

### 30. Revision-narrating prose

Watch for: sentences that narrate the draft's own history ("This chapter now focuses on", "As mentioned in an earlier version", explanations of what a passage replaced).

Left behind by AI-assisted revision loops. The reader has no earlier version.

Default action: Track change to describe the thing as it is.

### 31. Answering objections nobody raised

Watch for: defenses against criticism that appears nowhere in the text: "This isn't mainly about X", "I'm not saying", "I'm not arguing that", "To be clear, this doesn't mean", "Don't get me wrong", "Some might say… but" with no such objection anywhere in the book.

The writer rebuts a critic who is not on the page, and the rebuttal displaces the claim itself. A direct negative claim ("the API is not thread-safe") is not this pattern; the tell is the unattributed defense of a point never stated plainly.

Default action: Track change. Delete the phantom objection and its rebuttal; state the claim directly. A defense anchored to a real counterargument (a cited critic, an earlier chapter's caveat) stays. For the one-sentence contrast form, see pattern 9.
Fix: "This isn't mainly about prompt length. The retrieval step is the bottleneck" becomes "The retrieval step is the bottleneck."

### 32. Rejecting fake alternatives

Watch for: an option no reader would weigh, introduced only to be dismissed in the same clause: "A tempting approach would be", "One might be tempted to", "An obvious approach would be", "It would be easy to just", "You might think… but", where the option never appears again.

The phantom option is drafting scaffolding left in the final text. It manufactures the look of considered judgment without doing any. One rejected option can be legitimate analysis; several short, unrelated rejections are the tell.

Default action: Track change. Cut the fake alternative and state the real constraint or choice directly. An alternative the book's readers genuinely face is analysis; leave it and give it a fair sentence.
Fix: "A tempting approach would be to rotate tokens by restarting the service nightly, but that would drop every active session. Rotation happens in place" becomes "Rotation happens in place; a restart would drop every active session."

## Group 6: Mechanical artifacts of humanizer passes

Debris left by automated de-slopping tools. All of it is unambiguous. Sweep for these with grep before reading for prose; they hide in clean-looking paragraphs.

### 33. Stranded punctuation from dash conversion

Watch for: ",," sequences, ", ," patterns, a comma followed by a capitalized clause where a dash was mechanically swapped out, commas that break the sentence's grammar.

Default action: Track change. Read the sentence aloud and restore working punctuation.

### 34. Double spaces

Watch for: two or more spaces between sentences or words. Grep: `  ` (two spaces).

Default action: Track change to single spaces.

### 35. Broken list structure

Watch for: orphaned bullet or number markers, items that lost their markers, indentation drift within one list, a list interrupted by a stray paragraph.

Default action: Track change to restore the list; comment if it is unclear whether the passage should be a list or prose.

### 36. Quote and apostrophe mixing

Watch for: straight and curly quotes in the same paragraph, straight apostrophes inside curly-quoted text, unpaired smart quotes. Grep for `"` and `'` in a smart-quote manuscript.

Default action: Track change to the style-sheet standard (smart quotes by default, pattern 15).

## False positives: what not to flag

A clean human writer trips several of these patterns without any machine involvement. Look for clusters, never isolated hits.

- Polish. Perfect grammar and consistent style mean the writer is good or was edited, nothing more.
- Formal or academic vocabulary used correctly. The tell is the specific overused words in pattern 7, never fancy words in general.
- One em dash, used well.
- One short emphatic sentence.
- A single "however", "additionally", or "moreover". These are tells only in pileups.
- Genuine triads. Three items that each carry weight are rhetoric working as intended.
- Passive voice with a justified missing actor.
- Watched phrases inside quotations, titles, or text that discusses the phrase itself. Never edit quoted material.
- Dry prose. Machine prose has specific tells; dryness without them is just a dry writer.
- Deliberate repeated openings that build pressure ("She came. She saw. She conquered."). Pattern 11 targets repetition that adds nothing.
- Real scope statements and disclaimers: legal or safety notices, corrections, a named critic answered in full, FAQ answers. Pattern 31 targets only the unanchored defense.
- Real alternatives the reader genuinely faces (a design choice weighed, a route not taken and explained). Pattern 32 targets only the phantom kind, dismissed in a clause and never mentioned again.

One instance means nothing. An em dash plus a rule of three plus "vibrant tapestry" plus a recap ending in the same section is a confession.

## Signs of human writing: preserve these

These are evidence of a person on the page. Over-editing them destroys the manuscript's best asset, and every one belongs on the style sheet under author voice notes.

- Specific, hard-to-fabricate detail: a real address, an odd quote, "the lawyer who worked upstairs from my dentist". Machines round specifics off; people hoard them.
- Mixed feelings and unresolved tension: "mostly good, and it still bothers me". Machines default to clean takes.
- Era-bound references, slang, and in-jokes that date to a specific year and scene.
- Deliberate fragments and rhythm choices the author can defend.
- Genuine asides, parentheticals, and self-corrections.
- Distinctive vocabulary, bluntness, humor, and admitted uncertainty.
- Real variety in sentence length, including the occasional too-long sentence that works.
- Paragraphs of genuinely different sizes, including the one-sentence paragraph that earns its line.
- Conclusions that stop early instead of recapping.
- Contractions and register that match how the writer talks.
- Willingness to criticize by name and to leave a judgment unbalanced.
- Proper nouns with anchors: surnames, places, years, product versions.

When an edit must insert text, the insertion should carry these qualities too, in the author's register. An insertion that is smoother, more formal, and more evenly paced than the page around it reads as a seam.

## Editing principles

These govern how the catalog is applied. They come from the discipline of minimum intervention, and they are what separates an editor from a rewriter.

- **Minimum effective edit.** The smallest change that fixes the instance. If a sentence works, leave it alone, even if you would have written it differently.
- **Proportionality.** Edit density must track slop density. A clean paragraph gets no edits; do not polish for uniformity or make every paragraph equally tidy.
- **Leave strong sentences alone.** A strong human sentence adjacent to a weak machine one is the manuscript's voice showing through. Protect it.
- **The portability test.** If a sentence could sit unchanged in any book on any subject, it carries no information about this one. Cut it or make it specific, using material already in the manuscript.
- **Fix the instance, flag the habit.** Track-change the individual occurrence; when a pattern recurs, one comment on the pattern serves the author better than ten identical annotations.
