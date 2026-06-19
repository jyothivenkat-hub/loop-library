# Survey open-text coding loop

> Turn a pile of free-text answers into clean categories with a small catch-all.

**Goal:** Every open-ended response is categorized, and the catch-all "other" bucket holds under 5%.

- **Trigger:** After a survey with free-text questions closes.
- **Action:** Read responses, assign each to a category, and when "other" gets too big, split it into new categories.
- **Proof:** A category breakdown with counts and percentages, plus example responses per category.
- **Memory:** The category list so far, so the agent reuses categories instead of inventing duplicates.
- **Stop condition:** 100% of responses categorized, "other" under 5%.

## Starter prompt

```
Here are the open-text responses from my survey. Categorize every response. Start
with whatever categories emerge, and whenever the "other" bucket exceeds 5% of
responses, split it into new named categories and re-sort. Reuse existing categories,
do not create near-duplicates. Show a breakdown with counts, percentages, and two
example responses per category. Stop when every response is categorized and "other"
is under 5%.
```
