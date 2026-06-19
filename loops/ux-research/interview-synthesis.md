# Interview synthesis loop

> Code every transcript against your questions, with evidence behind every theme.

**Goal:** Every transcript is coded against the research questions, and every theme is backed by at least two quotes from different participants.

- **Trigger:** After a round of interviews is transcribed.
- **Action:** Read a transcript, tag segments against the research questions, group tags into themes.
- **Proof:** A theme table where each row lists supporting quotes and which participant said them.
- **Memory:** Themes already found, so later transcripts add evidence instead of starting over.
- **Stop condition:** All transcripts coded, every theme has two or more quotes from different participants.

## Starter prompt

```
Here are [N] interview transcripts and my research questions. Code each transcript:
tag segments against the questions, then group tags into themes. Build a theme table
where every row lists its supporting quotes and the participant who said each one.
A theme only counts if it has at least two quotes from two different participants.
Process all transcripts. Stop when every transcript is coded and every theme meets
the two-quote, two-participant bar. Flag any single-source patterns separately so I
can decide whether to keep them.
```
