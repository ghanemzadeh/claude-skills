# AI-prose pattern catalog

Read this file before editing the first chunk. It lists the patterns that mark a manuscript as machine-drafted, what each looks like, and what an editor does about each one inside a track-changes workflow.

Two rules govern every entry:

1. **This is surgery, not regeneration.** Fix each instance with the smallest edit that works. Never rewrite a passage wholesale and never run text through another generation pass.
2. **Never fabricate.** An edit may not introduce any fact, name, number, date, quote, or source that is not already in the manuscript or its citations. When a sentence needs information the manuscript does not contain (a source for a vague claim, a date for a hedge), the correct move is a query comment to the author.

## Why machine prose reads the way it does

A language model writes the most likely next word, so by default it makes the choice that suits the widest range of readers and subjects. A human writer chooses for one reader and one subject, and their choices come out uneven and specific. Every pattern below is a form of that default choice: a sentence that stages importance instead of adding a fact, a shape applied by rule (triads, dashes, bold labels, clipped sentences), an ordinary fact dressed up, chat and drafting leftovers, or background re-explained to a reader who already has it.

Two tests follow. Every sentence that survives the edit should give the reader something they did not already have, from earlier in the book or from common knowledge. And a tell weighs in proportion to how rarely a careful writer would make that choice on purpose. Word habits change with each model release; the structural habits persist, so read for shape first and vocabulary second.

## How to read an entry

- **Watch for** lists trigger words or shapes. All quoted material in this file is an example of the problem, kept for recognition. Do not flag this file's own examples.
- **Default action** is one of:
  - *Track change*: the fix is unambiguous; make it.
  - *Comment*: judgment call, missing information, or a pattern worth the author's attention; query, do not silently fix.
  - *Cover letter*: structural, out of scope for the edit itself; note it in the editorial cover letter.
  - *Leave*: within dose, or a legitimate stylistic choice.
- **Dose** appears where a pattern is only a problem in aggregate. Track tallies per chapter in your working notes. One instance of most of these patterns is ordinary writing; the tell is density.
- **Strength.** The strongest tells justify an edit on one sighting: unearned contrasts (9), chat residue (18, 20), staged run-ups (23), significance narration and deep-sounding sayings (24), kickers and one-line closers (26), and arguing with no one (31, 32). Patterns marked *weak alone* need company from other tells in the same passage before they count as evidence of machine drafting; they may still deserve an edit on ordinary editorial grounds.

## Group 1: Content patterns

### 1. Significance inflation

Watch for: "marks a pivotal moment", "stands as a testament", "underscores the importance", "reflects broader trends", "setting the stage for", "indelible mark", "key turning point", "evolving landscape", "enduring legacy", "plays a key role", "shaping the".

Statements that puff up an event or detail by tying it to sweeping importance. The sentence usually survives with the inflation cut. The same move works at three scales: a phrase, a stock "challenges and outlook" section (pattern 6), and a send-off paragraph (pattern 28).

Default action: Track change. Delete the inflating clause; keep the factual core.
Fix: "The institute was established in 1989, marking a pivotal moment in regional statistics" becomes "The institute was established in 1989."

### 2. Notability padding

Watch for: lists of media outlets with no context ("has been cited in the Times, the BBC, and the Financial Times"), follower counts, "written by a leading expert".

Default action: Track change if one citation in the list carries real context in the manuscript (keep that one, cut the roll call). Comment if none do: ask the author which mention matters and what was actually said. Do not invent the context.
Dose: a single contextualized citation is fine; the roll call is the tell.

### 3. Superficial "-ing" analysis

Watch for: trailing participle clauses that pretend to explain: "…, highlighting", "…, reflecting", "…, symbolizing", "…, showcasing", "…, ensuring", "…, fostering", "…, emphasizing", "…, underscoring", "…, encompassing", "…, cultivating", "…, contributing to".

The clause asserts meaning the sentence has not earned. Cutting it almost never loses information. Hanging the clause on a named source ("Ebert praised the score, highlighting its lasting influence") does not make the claim true; check that the source said it.

Default action: Track change. Delete the clause, or promote it to its own sentence if the manuscript elsewhere supports the claim.
Fix: "The palette uses blue and gold, reflecting the community's deep connection to the land" becomes "The palette uses blue and gold." If the connection is real and sourced in the manuscript, state it as its own sourced sentence.

### 4. Promotional language

Watch for: "vibrant", "nestled", "breathtaking", "renowned", "stunning", "rich cultural heritage", "boasts", "in the heart of", "must-visit", "groundbreaking" (figurative), "commitment to excellence", "profound", "exemplifies", "featuring", "diverse array".

Ad copy in the middle of nonfiction. The neutral version is nearly always shorter. Newer models are subtler: the copy is merely relentlessly upbeat, every company "innovative", every outcome a success. Honest negativity is a human signal (see "Signs of human writing").

Default action: Track change to the neutral statement.
Fix: "Nestled in the breathtaking region of Gonder, the town boasts a rich heritage" becomes "The town is in the Gonder region."

### 5. Vague attribution and generic specifics

Watch for: "experts argue", "observers have noted", "industry reports suggest", "studies show", "critics say", "it is widely believed", with no named source.

Watch for, second form: detail that gestures at specificity without containing any. Anecdote characters with a first name and a job title only ("Sarah, a marketing manager"), "a mid-sized company in the Midwest", suspiciously round numbers with no source, an example that would fit any book on the subject unchanged. Generated anecdotes cluster on the same stock names and settings; a real person comes with a surname, a place, a year, or an odd particular.

Both forms need information only the author has, so this is the pattern an editor must never fix directly. A plain claim with no citation is not this pattern; most writing is unsourced. The tell is the gesture at an authority or a specific that is not there.

Default action: Comment, always. For attribution: "Which experts? Needs a named source or a cut." For a generic specific: "Is this a real person or company? If real, an anchoring detail (full name, place, year) would carry it. If illustrative or composite, say so in the text." If the manuscript cites a real source nearby, a track change attaching the claim to that source is allowed. The specificity must come from the author; never invent it.
Dose: none. Every unsourced attribution and every generic specific gets flagged.

### 6. Formulaic sections

Watch for: "Challenges and Future Prospects", "Despite these challenges…", "Future Outlook", "Legacy", "Awards and Recognition", "Conclusion" sections that restate the chapter, any section whose structure could be pasted into a different book unchanged.

Default action: Comment on the section plus a cover-letter note. Restructuring is out of scope, but the author should know the section reads as boilerplate.

## Group 2: Language patterns

### 7. AI vocabulary

Watch for, tier one (near-certain tells, cut or replace on sight): delve, deep dive, tapestry (abstract), landscape (abstract), realm, beacon, interplay, testament, underscore (verb), showcase (verb), foster, garner, bolstered, gate/gated/gating (figurative; established technical senses such as feature gating stay), elevate, embark, harness, supercharge, leverage (verb), utilize, facilitate, empower, streamline, multifaceted, paramount, ever-evolving, meticulous/meticulously, paradigm shift, game changer, transformative, cutting-edge, robust (figurative).

Watch for, tier two (fine alone, a tell in clusters): crucial, pivotal, key (adjective), vital, enduring, intricate/intricacies, vibrant, enhance, highlight (verb), valuable, notably, additionally (especially opening a sentence), moreover, align with, emphasize, quietly (as drama: "quietly became").

Watch for, tier three (recent models, mid-2026 on; ordinary words, so a tell only in dense clusters alongside other patterns): challenge, clearer, dependable, echoed, matters ("That matters", "this is what matters"), practical, prioritize, steady, universally.

Vocabulary drifts with every model release ("delve" peaked in 2023 and has nearly vanished), so a page free of these words proves nothing. Take each entry literally: a word on the list does not put its synonyms on the list, and a formal word outside it is not a tell.

Default action: Track change to the plain word ("use" for "utilize", "build" for "foster", "run through" for "delve into"). Tiers two and three: leave singles, thin clusters. Empty adverbs ("actually", "literally", "simply") live in pattern 21.
Dose: tier one, zero tolerance. Tier two, flag when three or more land in a paragraph. Tier three, flag only when the cluster sits on a page that already shows structural patterns.

### 8. Copula avoidance

Watch for: "serves as", "stands as", "functions as", "operates as", "marks", "represents" (for "is"), "boasts", "features", "offers", "maintains" (for "has"), "refers to".

Simple *is* and *has* phrases ("there is a", "it has a") are measurably more common in human prose than in generated text. So are plain verbs over stiff ones: "wrote" not "authored", "used" not "utilized", "died" not "passed away".

Default action: Track change to "is", "are", "has".
Fix: "The gallery serves as the exhibition space and boasts four rooms" becomes "The gallery is the exhibition space and has four rooms."

### 9. Negative parallelism and binary contrast

Watch for: "It's not just X. It's Y.", "not only… but also", "This isn't about X, it's about Y", the reversed form "Y rather than X", the contrast split across sentences ("This does not mean X. It means Y."), negative listing ("not X, not Y, but Z"), tailing negation fragments ("no guessing", "no wasted motion").

The negative half names something nobody claimed, so the positive half sounds bigger. It adds weight without adding a claim. The information is in Y. State Y. This is currently the single most frequent structural tell in model prose; it also survives rewrites more often than any other pattern.

Keep a contrast when the negative half corrects a belief the book's reader actually holds (a misconception the manuscript names or the field is known for), or when both halves carry information. "Not only… but also" is common in human writing and is the weakest form.

Default action: Track change, unless one of the keep conditions holds.
Dose: kept contrasts go on the tally. When a chapter keeps more than two, comment on the chapter's pattern once ("third 'not just X' in this chapter; I've rebuilt two, flagging the shape for your eye").
Fix: "This does not mean every choice is equal. It means no outside system confirms which choice is right" becomes "No outside system confirms which choice is right, though the choices still have different consequences."

### 10. Rule of three

Watch for: chains of three parallel items where two would do or where the third is padding ("innovation, inspiration, and industry insights"), triple noun-phrase appositions ("the X, the Y, the Z"); at paragraph scale, three parallel examples in a row, or three short parallel sentences followed by a lesson ("A career can look promising and fail. A relationship can feel important and end. A skill can take years and remain useless. These decisions rarely explain themselves.").

Genuine triads exist; the tell is recurrence and padding. It is stronger where nobody would bother with a flourish: a caption, a transition, a list of examples.

Default action: Track change when a member is clearly filler (cut to two, or to the one that matters). At paragraph scale, merge two of the parallel sentences or develop the strongest example; check that every fact in the cut members survives somewhere. Leave real triads.
Dose: flag when triads recur within a few pages.

### 11. Synonym cycling and repeated sentence openings

Watch for: the same referent renamed each mention ("the protagonist… the main character… the central figure… the hero"); consecutive sentences opening on the same subject and shape ("She noted the door. She noted the lock on it. She filed both away.").

Cycling fakes variety the prose does not need; repeated openings drop variety it does. Both come from handling repetition by rule instead of by ear.

Synonym cycling is now *weak alone* as evidence of machine drafting: it was common in 2023-era models and has faded, and many writers, especially those schooled in languages that teach against repeating a word, cycle on purpose. It remains an editing problem in nonfiction, where a renamed referent can read as a new one, so fix it on clarity grounds and do not cite it as a machine tell.

Default action: Track change. For cycling, repeat the right word; repetition of a precise term is correct style. For repeated openings, merge the sentences, change one subject, or open one on the action. Fix the shape, not the repeated word; the surviving sentence may still start with "She". Deliberate repetition that builds pressure ("She came. She saw. She conquered.") is voice. For rhythm problems at passage scale, see pattern 27.

### 12. False ranges

Watch for: "from X to Y" where X and Y sit on no meaningful scale ("from the singularity of the Big Bang to the enigmatic dance of dark matter").

*Weak alone.* Humans write false ranges too, and current models rarely do; treat it as a precision edit only.

Default action: Track change to a plain list of what is actually covered.

### 13. Passive voice and subjectless fragments

Watch for: actorless constructions ("mistakes were made", "the decision was reached"), verbless fragments doing a sentence's job ("No configuration needed.").

Passive voice is legitimate when the actor is unknown or beside the point. The tell is passives that hide an actor the sentence needs, and fragment stacks. *Weak alone.* A related habit: inanimate things doing human verbs ("the decision emerged", "the data wants"); name who acted when the manuscript says.

Default action: Track change when the active version is clearer and the actor is in the manuscript. Leave justified passives.

## Group 3: Style patterns

Where this catalog diverges from humanizer: humanizer edits web prose, bans em dashes outright, and treats curly quotes as a weak tell. This skill edits book manuscripts to publishing standards, where both are legitimate. The rules below are calibrated for that context; they treat density, not existence, as the tell.

The evidence has moved this way too. Wikipedia's "Signs of AI writing" guide now files em-dash overuse under historical indicators (2022 to September 2026): the newest models are tuned to avoid dashes entirely, and the side effect is prose built almost only from commas and periods, which has become its own tell (pattern 35). A blanket dash ban now pushes a manuscript toward the newer machine signature. The same guide notes that curly quotes alone prove nothing, since Chicago-style publishing and every major word processor produce them.

### 14. Em-dash density

Watch for: more than one em dash per paragraph, dashes appearing in consecutive paragraphs, any sentence carrying two or more; spaced em dashes or typed double hyphens (" -- ") in a manuscript whose convention is unspaced, since generated dashes usually arrive spaced and often mark pasted passages.

Chicago permits em dashes and this skill's default style keeps them, unspaced. Density is still a machine-drafting tell in text from 2022 to 2026 models; one dash, used well, is *weak alone*.

Default action: Track change any sentence with two or more em dashes (read aloud, rebuild with commas, a colon, parentheses, or a sentence break). Vary the replacements: if every dash becomes a comma, the passage trades one tell for another (pattern 35). For paragraph-level clusters, track-change the weakest dashes and add one comment noting the pattern. Spacing and double-hyphen fixes are style-sheet conformance; sweep them with grep. Record the author's deliberate dash style on the style sheet; a confirmed heavy-dash voice overrides this rule, per the style sheet.
Dose: a lone em dash used well is good prose. Leave it.

### 15. Quotation mark policy

Watch for: straight quotes in a manuscript that should ship with smart quotes; apostrophes rendered as straight ticks.

Book publishing uses smart (curly) quotes. Here they are a requirement, never a tell. Mixing is the artifact; see pattern 40 for the mechanical sweep.

Default action: Track change straight to smart, per the style sheet.

### 16. Decorative emphasis

Watch for: mechanical boldface on key terms, bullet lists whose items open with a bolded header and a colon, emoji or decorative arrows (→) in headings or lists, bullets carrying what should be a prose paragraph, typographic shouting (one word in ALL CAPS, "every. single. day."), stray Markdown (asterisks, pound signs) surviving from a chat window.

Rare in trade nonfiction, common in AI-drafted chapters that began life as an outline.

Default action: Comment first (formatting can be a design decision the author or publisher owns); track change when the author has already confirmed prose conventions on the style sheet.

### 17. Heading conventions

Watch for: title case where the book's convention is sentence case (or drift between the two), a heading followed by a one-line warm-up that restates the heading before the content starts, a horizontal rule or ornament between every section where the design calls for none, subheads written for effect rather than content ("The decision, on one screen") across a whole chapter.

Default action: Track change case drift to the style-sheet convention. Track-change delete restater lines; the section should open with its first real sentence. Clever subheads are a legitimate trade-nonfiction convention; when every subhead in a chapter is a teaser that hides what the section holds, comment once and suggest naming the content.

## Group 4: Communication patterns

Chat residue: text written to a user that survived into the manuscript. All of it is a track-change deletion.

### 18. Chatbot artifacts

Watch for: "I hope this helps", "Let me know if", "Would you like me to", "Want me to", "Should I continue?", "Certainly!", "Of course!", "Here is an overview of", "Here's a revised version", "In this section, we will".

This is the most certain tell in the catalog and the easiest to miss when it wraps real content, so scan chapter openings and endings for it specifically.

Default action: Track change, delete. If deletion leaves a hole, open the section on its first substantive sentence.

### 19. Knowledge-cutoff disclaimers and speculative gap-filling

Watch for: "as of this writing" (when nothing dates it), "while specific details are scarce", "based on available information", "not widely documented", "not publicly disclosed", "in the available sources", "maintains a low profile", "keeps personal details private", "likely grew up", "it is believed that".

Two forms: the disclaimer that narrates a research gap, and the invented filler that papers over one. Both are dangerous in nonfiction because the filler reads as fact.

Default action: Track change deletes the disclaimer framing. The underlying gap gets a comment: "Source for this? As written it's a guess dressed as fact." Never fill the gap yourself.

### 20. Sycophantic register

Watch for: "Great question", "You're absolutely right", reader-flattering asides ("as the savvy reader will have noticed").

Default action: Track change, delete.

## Group 5: Filler, hedging, and rhetoric

### 21. Filler phrases and empty adverbs

Watch for: "in order to", "due to the fact that", "at this point in time", "it is important to note that", "it's worth noting", "when it comes to", "at the end of the day", "in today's world", "going forward"; adverbs doing no work: "very", "really", "quite", "actually", "literally", "simply", "truly", "essentially", "fundamentally", "ultimately".

Default action: Track change. These are the first cuts in any compression pass.

These are compression targets, not machine tells. Ordinary intensifiers ("very"), qualifiers ("perhaps", "tends to"), and wordy constructions ("in order to", "the fact that") turn up measurably more often in human prose than in generated text. Cut them where they pad; never sweep a chapter to zero, because a page with none of them reads over-processed.

### 22. Hedge stacking

Watch for: multiple qualifiers on one claim ("could potentially possibly be argued that… might"); caveat tics accumulating across a passage: "to be fair", "it's also possible", "might arguably", "in some cases it may", "this is an inference".

One hedge is honesty; a stack is evasion. Revision loops add qualifiers a pass at a time until every claim sounds unsure. Keep the strongest single qualifier the claim deserves, and cut caveats that exist only to repair an earlier overstatement. *Weak alone*: a single "perhaps" or "tends to" is a human habit.

Default action: Track change to one hedge or none.

### 23. Throat-clearing and signposting

Watch for: "Let's dive in", "let's explore", "let's break this down", "now let's look at", "here's what you need to know", "without further ado", "heads up", "quick note", "before I forget"; conversational hooks used as fake-candid openers ("Honestly?", "Look,", "Here's the thing", "The thing is", "Let's be honest", "Real talk", "Let me be clear", "I'll be honest", "The uncomfortable truth is"); rhetorical setups ("What if I told you", "Think about it:", "Plot twist:", a self-answered "Question? Answer." pair).

The announcement can wear a casual register too ("one thing that bit me hard, so pay attention to this part:"). Remove the announcement, not just its formal tone.

Default action: Track change, delete; the paragraph starts at its first real claim. Leave "honestly" and "look" when they occur mid-sentence in a genuinely conversational voice; the tell is the standalone theatrical opener.

### 24. Authority tropes, faux-insight setups, and significance narration

Watch for: "the real question is", "at its core", "in reality", "fundamentally", "what really matters", "the deeper issue", "the heart of the matter"; "what most people miss", "what nobody tells you", "the part everyone gets wrong"; and, after a point has been made, commentary narrating its weight: "That last part matters more than it sounds", "This distinction matters", "The key point is", "As you can see", "Read that again", a redundant "In other words".

The setup puts ceremony before the point; the narration puts ceremony after it. Either way the sentence tells the reader the point matters instead of making it matter.

Default action: Track change. Keep the point, cut the ceremony. When the point does not read clearly without the aside, the fix belongs in the point's own sentence, built from support already in the manuscript.

### 25. Colon reveals

Watch for: a dramatic pause-and-reveal built on a colon ("The answer: nobody knows.", "One word: leverage.").

Default action: Track change into a plain sentence when the reveal adds no information. Leave a colon doing honest work (introducing a list, an explanation, a quotation).
Dose: one per chapter can be voice. A recurring cadence is a tell.

### 26. Aphorisms, kickers, and one-line closers

Watch for: "X is the Y of Z", "X is not a tool but a mirror", "X becomes a trap", "the language of", "the currency of", "the architecture of"; closing lines that reach for quotability ("In the end, the market wasn't buying software. It was buying belief."); a one-sentence paragraph that restates the paragraph before it ("That is the real win.", "Let that sink in."); the same closer shape after section after section; a sentence after an anecdote, example, or number that names what it just showed ("This shows the importance of preparation.", "The message was clear:", "It was a lesson in patience.").

Each of these asks the reader to pause on a point instead of adding to it. The explained example is especially common in AI-drafted nonfiction, because every anecdote gets a moral appended. A reader who just watched the example does not need it labeled.

Default action: Track change. Replace the formula with the concrete claim it gestures at. Delete kickers and restating closers outright and end on the last concrete point; do not rewrite a fake-profound line into a better metaphor. Cut the sentence that explains an example unless it adds a fact or consequence the example does not show. A short sentence that carries new information stays, however punchy.

### 27. Manufactured staccato and robotic rhythm

Watch for: runs of clipped fragments engineered for drama ("No aesthetic prior. No nostalgia. The old rules were gone."); paragraphs where every sentence has the same length and shape; every paragraph landing on a punchline; pages where sentence length barely varies; chapters whose paragraphs all run to the same size.

One short sentence for emphasis is human writing. A run of them is percussion. Uniformity is the same tell at document scale: a human page mixes a six-word sentence with a forty-word one, and a two-line paragraph with a half-page one, where generated pages average out. On a suspect page, count words per sentence (the pre-delivery checklist has a spot check); when most sentences land within a few words of the mean, read the page aloud before deciding anything. For the newer clamped form (every sentence between roughly 8 and 20 words, commas and periods only), see pattern 35.

Default action: Comment, usually. Rhythm rebuilds are voice-level judgment calls; propose the rebuild in a comment during calibration, then apply the agreed treatment as track changes in later chunks. Track change directly only when the fix is a simple merge of two fragments. For document-level monotony, comment during calibration and propose where the variance should come from: splitting one overlong sentence, merging two clipped ones, letting a short paragraph stand alone. Variance comes from cuts and merges of what is already there, never from padding.

### 28. Generic conclusions and recap endings

Watch for: "The future looks bright", "Exciting times lie ahead", "a major step in the right direction"; final paragraphs opening "In conclusion", "In summary", or "Overall"; chapter endings that summarize the chapter just read, sized like a term paper's.

Human conclusions run short; a chapter that has made its argument can simply stop.

Default action: Track change. Cut the send-off; end on the last concrete fact, takeaway, or forward action the manuscript actually supports. A recap that the author clearly built as a pedagogical device gets a comment instead.

### 29. Hyphenation drift in compound pairs

Watch for: compounds hyphenated in predicate position ("the report is high-quality", "the plan is long-term", "the process is well-documented").

Hyphenate attributive use ("a high-quality report"); drop the hyphen after the noun ("the report is high quality"). Compounds the dictionary always hyphenates ("cross-functional", "third-party", "self-aware") keep the hyphen in every position; check Merriam-Webster and the Chicago hyphenation table before cutting one. Uniform hyphenation everywhere is a machine habit, but *weak alone*.

Default action: Track change; record the convention on the style sheet.

### 30. Text that describes itself

Watch for: sentences that narrate the draft's own history ("This chapter now focuses on", "As mentioned in an earlier version", explanations of what a passage replaced); narration of how the text was assembled ("drawn from", "compiled from", "anything I couldn't confirm is flagged rather than guessed"); a description of a layout the reader can already see ("the table below compares", "this section is organized by decade").

Left behind by AI-assisted revision loops and by the model reporting its own method. The reader has no earlier version and does not need the workflow.

Books have legitimate versions of this: an introduction's roadmap, a note on sources, a methodology appendix, an edition preface. Leave those. The tell is the same narration scattered through body text. A single description of a table or figure is *weak alone*.

Default action: Track change to describe the thing as it is. Keep a source credit the reader can follow and a caveat that changes how the reader should use the information; cut the account of how the text was put together.

### 31. Answering objections nobody raised

Watch for: defenses against criticism that appears nowhere in the text: "This isn't mainly about X", "I'm not saying", "I'm not arguing that", "To be clear, this doesn't mean", "This is not to say", "Don't get me wrong", "Some might say… but" with no such objection anywhere in the book. Several unrelated defenses in a row are a stronger sign than one.

The writer rebuts a critic who is not on the page, and the rebuttal displaces the claim itself. A direct negative claim ("the API is not thread-safe") is not this pattern; the tell is the unattributed defense of a point never stated plainly.

Default action: Track change. Delete the phantom objection and its rebuttal; state the claim directly. A defense anchored to a real counterargument (a cited critic, an earlier chapter's caveat) stays. For the one-sentence contrast form, see pattern 9.
Fix: "This isn't mainly about prompt length. The retrieval step is the bottleneck" becomes "The retrieval step is the bottleneck."

### 32. Rejecting fake alternatives

Watch for: an option no reader would weigh, introduced only to be dismissed in the same clause: "A tempting approach would be", "One might be tempted to", "An obvious approach would be", "It would be easy to just", "You might think… but", where the option never appears again.

The phantom option is drafting scaffolding left in the final text. It manufactures the look of considered judgment without doing any. One rejected option can be legitimate analysis; several short, unrelated rejections are the tell.

Default action: Track change. Cut the fake alternative and state the real constraint or choice directly. An alternative the book's readers genuinely face is analysis; leave it and give it a fair sentence.
Fix: "A tempting approach would be to rotate tokens by restarting the service nightly, but that would drop every active session. Rotation happens in place" becomes "Rotation happens in place; a restart would drop every active session."

## Group 6: Document-level patterns

These survive sentence-level cleanup because every sentence can read fine on its own. They show up only across a page, a chapter, or the whole book.

### 33. Vague connection or association

Watch for: "associated with", "in association with", "connected to", "in connection with", "linked to", "tied to", where the actual relationship is known.

"He was associated with the company" hides whether he founded it, ran it, or consulted for it. The vague verb is the model declining to commit to a relationship.

Default action: Track change to the specific relationship when the manuscript or its citations state it ("He founded and conducts the orchestra"). When they do not, comment and ask; never pick a role. Statistical or scientific "associated with" (a correlation, stated as such) is precise usage; leave it.

### 34. Re-explaining what the reader already has

Watch for: a person re-introduced with full name and credentials in chapter after chapter; a coined term defined again from scratch; a chapter opening that recaps the previous chapter before starting its own; background the book already covered, rebuilt before the new point arrives, so the point lands last.

Chapters drafted in separate AI sessions each assume a reader with no context, because that suits the widest range of readers. A book's reader has read the earlier chapters. Every sentence should give them something they did not already have.

Default action: Track change re-introductions to the short form the style sheet sets (full name and credential at first mention in the book, or at first mention per chapter if that is the author's convention). Comment on recaps and rebuilt background, citing where the book already covered it: these may be deliberate signposting for readers who dip into chapters, which is the author's call. Cover-letter note when the pattern runs through the manuscript.

### 35. Clamped sentences and punctuation monotony

Watch for: pages built almost entirely from commas and periods, with no semicolons, colons, parentheses, or dashes where the author uses them elsewhere; sentence lengths held inside a narrow band (roughly 8 to 20 words) with no short punch and no long periodic sentence; every em dash in a passage converted to a comma.

The newest models are tuned to avoid em dashes and to keep sentences short, and humanizer tools that ban dashes produce the same result. Wikipedia's guide now lists heavy comma-and-period use with short, clamped sentences as a sign of recent model output. Human writers use the whole punctuation kit and let sentence length swing.

Default action: Comment during calibration with the page's numbers (the pre-delivery checklist's spot check prints them) and the author's baseline for comparison. Once the author agrees on the treatment, apply it as track changes: restore a semicolon or dash where two clauses are tightly bound, merge two clipped sentences, let one long sentence run. Every change rearranges what is already there; never pad a sentence to lengthen it.
Dose: measured against the author's voice baseline. Some authors write spare comma-and-period prose by choice; for them the pattern does not apply.

### 36. Style seams

Watch for: a passage or chapter whose register, polish, spelling variety (US forms in a UK manuscript), dash spacing, quote style, or vocabulary breaks sharply from the manuscript around it; a section noticeably more fluent and less specific than the author's other pages.

A seam usually marks text pasted in from a chat window or regenerated in isolation. It is the book-length version of Wikipedia's "pronounced shift in writing style" sign.

Default action: Fix mechanical conformance (spelling variety, dash spacing, quotes) as track changes per the style sheet. Comment on the register shift and name it in the cover letter. Never normalize the author's own pages toward the seam; the seam moves toward the author.

## Group 7: Mechanical artifacts of humanizer passes

Debris left by automated de-slopping tools. All of it is unambiguous. Sweep for these with grep before reading for prose; they hide in clean-looking paragraphs.

### 37. Stranded punctuation from dash conversion

Watch for: ",," sequences, ", ," patterns, a comma followed by a capitalized clause where a dash was mechanically swapped out, commas that break the sentence's grammar, a comma splice where a dash used to join two independent clauses.

Default action: Track change. Read the sentence aloud and restore working punctuation: a period, a semicolon, a colon, parentheses, or the original dash if the style sheet allows it. When a whole passage was converted the same way, also see pattern 35.

### 38. Double spaces

Watch for: two or more spaces between sentences or words. Grep: `  ` (two spaces).

Default action: Track change to single spaces.

### 39. Broken list structure

Watch for: orphaned bullet or number markers, items that lost their markers, indentation drift within one list, a list interrupted by a stray paragraph.

Default action: Track change to restore the list; comment if it is unclear whether the passage should be a list or prose.

### 40. Quote and apostrophe mixing

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
- Mixed registers. Casual and formal side by side, or clinical and emotional in one paragraph, is how many technical writers, younger writers, and co-authored books sound.
- Transition words, ordinary hedges, and intensifiers in isolation ("however", "perhaps", "tends to", "very"). Human prose carries more of these than generated prose does.
- Unsourced claims. Most writing is unsourced; pattern 5 targets only vague authority.
- Smart quotes. Chicago-style publishing and every major word processor produce them.
- Text written before November 30, 2022. It is not AI-drafted, whatever it looks like. When the author can say which chapters predate AI assistance, those are the voice baseline.

Neither readers judging by feel nor detector scores are reliable on their own; both misfire on skilled human writers. Clusters of named patterns are the only evidence worth acting on. One instance means nothing. An em dash plus a rule of three plus "vibrant tapestry" plus a recap ending in the same section is a confession.

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
- The full punctuation kit, used the way this author uses it: semicolons, parentheses, colons, the occasional dash.
- Plain verbs and simple syntax: "wrote", "used", "tried", "died"; "there is", "it has". Generated prose reaches for "authored", "utilized", "attempted", "passed away", and "serves as".
- Definite statements where the manuscript supports them: "the first", "the only", "one of the best". Generated prose hedges these away.
- A voice that matches the author's writing from before AI assistance, where any exists.

When an edit must insert text, the insertion should carry these qualities too, in the author's register. An insertion that is smoother, more formal, and more evenly paced than the page around it reads as a seam.

## Editing principles

These govern how the catalog is applied. They come from the discipline of minimum intervention, and they are what separates an editor from a rewriter.

- **Minimum effective edit.** The smallest change that fixes the instance. If a sentence works, leave it alone, even if you would have written it differently.
- **Proportionality.** Edit density must track slop density. A clean paragraph gets no edits; do not polish for uniformity or make every paragraph equally tidy.
- **Leave strong sentences alone.** A strong human sentence adjacent to a weak machine one is the manuscript's voice showing through. Protect it.
- **Add something or go.** Every sentence that survives should give the reader something they did not already have, from earlier in the book or from common knowledge. This is the test behind patterns 24, 26, 28, and 34.
- **The portability test.** If a sentence could sit unchanged in any book on any subject, it carries no information about this one. Cut it or make it specific, using material already in the manuscript.
- **Fix the instance, flag the habit.** Track-change the individual occurrence; when a pattern recurs, one comment on the pattern serves the author better than ten identical annotations.
- **Fix the shape.** Swapping a flagged word for a synonym leaves the shape that made it machine-like. If a sentence still reads generated after the patch, rebuild it around its main point, inside the same paragraph and with the same facts.
- **Shape edits drop facts.** Cutting a triad, rebuilding a dash, or turning a bold-label list into prose is where a fact, a ranking, or an "at the same time" relation most often goes missing. Check each one against the original before moving on.
- **Second sweep for survivors.** After the edit, search the chunk again for the patterns that most often survive a rewrite: contrasts (9), closers and kickers (26), triads (10), dashes (14), and bold labels (16).
