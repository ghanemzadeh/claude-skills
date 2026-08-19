# Pre-delivery checklist

Run this before delivering each chunk. Every line is pass or fail. A failed line means fix the chunk and run the checklist again; never deliver-and-note.

## Voice

1. Read one edited paragraph aloud (or subvocalize it). Does it sound like the author, at the author's level of polish?
2. Would the author recognize the edited chunk as their own writing? Check the edits against the author voice notes on the style sheet.
3. Did every deliberate tic listed in the voice notes survive (fragments, sentence-opener And/But, specific vocabulary)?

## Proportionality

4. Does edit density track slop density? Heavily edited paragraphs should be the ones that had problems.
5. Did clean paragraphs pass through untouched? If a paragraph with no catalog hits carries edits, justify each one or revert it.
6. Is the cutting proportional? No passage compressed so hard it lost character or a concrete detail.

## No new slop

7. Extract the inserted text (every `w:ins` run) and read it against `ai-prose-patterns.md`. Insertions are where the editor's own machine habits leak in.
8. Inserted text contains no em dashes beyond the style-sheet allowance, no pattern-7 vocabulary, no filler phrases.
9. Inserted sentences vary in length and shape; no run of same-shape sentences was created by the edits.
10. Rhythm survives at page scale. On the most heavily edited page, sentence lengths still vary. Spot check:

    ```bash
    unzip -p manuscript_edited.docx word/document.xml \
      | sed -e 's|<w:delText[^>]*>[^<]*</w:delText>||g' -e 's|</w:p>|\n|g' -e 's/<[^>]*>//g' \
      | tr '.!?' '\n' \
      | awk 'NF>0 {n++; s+=NF; w[n]=NF}
          END {m=s/n; for(i=1;i<=n;i++) v+=(w[i]-m)^2;
          printf "sentences %d, mean %.1f, sd %.1f\n", n, m, sqrt(v/n)}'
    ```

    The count is crude (abbreviations split as short fragments). A standard deviation under about a third of the mean says the page may have flattened; reread it aloud. The number prompts a reread, never an edit by itself.
11. Register match. Insertions follow the author's baseline: contractions where the author contracts, bluntness where the author is blunt. No "do not" inserted into a manuscript that writes "don't".
12. Endings are recap-free. Chapter endings in this chunk close on a concrete point; no recap or send-off survived the edit (pattern 28) and none was introduced.

## No fabrication

13. Every fact, name, number, date, and source in inserted text already existed in the manuscript or its citations.
14. Every unverifiable claim encountered got a comment, never a silent fix or an invented specific.

## Dose budgets

15. Per-chapter tallies are current: negative parallelisms kept, rule-of-three instances kept, sentence-opener And/But clusters, em dashes remaining, colon reveals kept.
16. Every over-budget pattern either got fixed or carries a comment flagging it for the author.

## Mechanics

17. The repacked docx passes `unzip -t` and opens cleanly (Word, LibreOffice, or Pages).
18. Tracked changes appear in the Review pane and are individually acceptable and rejectable.
19. All `w:id` values are unique across the document; the running counter's high-water mark is recorded in the working notes.
20. Running wordcount delta is on track for the agreed compression target.
21. Style sheet, names list, and facts list reflect every decision made in this chunk.
22. Every judgment call is a comment; nothing ambiguous was changed silently.
23. Grep sweeps for mechanical artifacts came back clean: double spaces, ",," sequences, straight quotes in smart-quote text, orphaned list markers.
