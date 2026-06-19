# Survey open-text coding

> Turn a pile of free-text answers into clean categories with a small catch-all.

## Goal (the what)

- **Objective:** Categorize every open-ended survey response.
- **Success criteria:** 100% of responses categorized, with the catch-all "other" bucket under 5%.
- **Constraints:** Reuse existing categories, do not create near-duplicates.
- **Context:** The survey question and the full set of responses.

## Loop (the how)

- **Think:** Read a response, decide which category it fits.
- **Act:** Assign it, or when "other" gets too big, split it into new named categories.
- **Observe:** Check the size of the "other" bucket as a percentage.
- **Reflect / Plan:** Merge duplicate categories, re-sort responses affected by a new category.
- **Stop when:** Every response is categorized and "other" is under 5%.

## Starter prompt

```
Here are the open-text responses from my survey. Categorize every response. Start
with whatever categories emerge, and whenever "other" exceeds 5%, split it into new
named categories and re-sort. Reuse existing categories, no near-duplicates. Show a
breakdown with counts, percentages, and two example responses per category. Stop when
every response is categorized and "other" is under 5%.
```
