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
10. Rhythm and punctuation survive at page scale. On the most heavily edited chapter, sentence lengths still vary and the punctuation range still matches the voice baseline. Spot check (run it on the author's baseline too, for comparison):

    ```bash
    unzip -p manuscript_edited.docx word/document.xml \
      | sed -e 's|<w:delText[^>]*>[^<]*</w:delText>||g' -e 's|</w:p>|\n|g' -e 's/<[^>]*>//g' \
      > edited.txt

    tr '.!?' '\n' < edited.txt \
      | awk 'NF>0 {n++; s+=NF; w[n]=NF; if (NF>=8 && NF<=20) band++; if (NF<6) sh++; if (NF>30) lg++}
          END {m=s/n; for(i=1;i<=n;i++) v+=(w[i]-m)^2;
          printf "sentences %d, mean %.1f, sd %.1f, in 8-20 band %d%%, under 6 words %d, over 30 words %d\n",
            n, m, sqrt(v/n), 100*band/n, sh, lg}'

    words=$(wc -w < edited.txt)
    for mark in ';' ':' '(' '—' ','; do
      grep -o -- "$mark" edited.txt | wc -l \
        | awk -v m="$mark" -v w="$words" '{printf "%s per 1,000 words: %.1f\n", m, 1000*$1/w}'
    done
    ```

    The counts are crude (abbreviations and decimals split as short fragments; colons include ratios and times). Three readings say the chapter may have flattened: a standard deviation under about a third of the mean; nearly every sentence inside the 8-20 band with none under 6 or over 30 words (pattern 35); semicolons, parentheses, and dashes near zero where the baseline uses them. Any of these prompts a reread aloud, never an edit by itself.
11. Register match. Insertions follow the author's baseline: contractions where the author contracts, bluntness where the author is blunt. No "do not" inserted into a manuscript that writes "don't".
12. Endings are recap-free. Chapter endings in this chunk close on a concrete point; no recap or send-off survived the edit (pattern 28) and none was introduced.
13. Dash rebuilds vary. Where em dashes were removed, the replacements differ (period, semicolon, colon, parentheses, comma) as each sentence needs; no passage had every dash turned into a comma.
14. Survivors swept. A second search of the edited chunk found no surviving unearned contrasts (9), restating closers or explained examples (26), padded triads (10), dash clusters (14), or bold-label lists (16).
15. Nothing re-explained. No person, term, or argument is re-introduced at full length after the book already introduced it, unless the author confirmed the signposting (pattern 34).

## No fabrication

16. Every fact, name, number, date, and source in inserted text already existed in the manuscript or its citations.
17. Shape edits kept their facts. Every cut triad, rebuilt dash, and list turned to prose still carries each fact, ranking, and "at the same time" relation from the original.
18. Every unverifiable claim encountered got a comment, never a silent fix or an invented specific.

## Dose budgets

19. Per-chapter tallies are current: negative parallelisms kept, rule-of-three instances kept, sentence-opener And/But clusters, em dashes remaining, colon reveals kept.
20. Every over-budget pattern either got fixed or carries a comment flagging it for the author.

## Mechanics

21. The repacked docx passes `unzip -t` and opens cleanly (Word, LibreOffice, or Pages).
22. Tracked changes appear in the Review pane and are individually acceptable and rejectable.
23. All `w:id` values are unique across the document; the running counter's high-water mark is recorded in the working notes.
24. Running wordcount delta is on track for the agreed compression target.
25. Style sheet, names list, and facts list reflect every decision made in this chunk.
26. Every judgment call is a comment; nothing ambiguous was changed silently.
27. Grep sweeps for mechanical artifacts came back clean: double spaces, ",," sequences, straight quotes in smart-quote text, orphaned list markers, spaced em dashes or typed " -- " in an unspaced-dash manuscript.
