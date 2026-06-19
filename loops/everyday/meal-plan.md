# Weekly meal plan loop

> A week of dinners that respects your real constraints, not a generic list.

**Goal:** A 7 day dinner plan where no main ingredient repeats and every meal fits a 30 minute cook time.

- **Trigger:** Start of the week, or when you are out of ideas.
- **Action:** Draft the week, then check each day against the two rules and fix violations.
- **Proof:** A table with the meal, main ingredient, and cook time per day.
- **Memory:** Mains already used this week, plus anything you said you disliked.
- **Stop condition:** Seven days, zero repeated mains, every meal under 30 minutes.

## Starter prompt

```
Plan 7 dinners for me. Rules: no main ingredient repeats across the week, and every
meal cooks in under 30 minutes. Draft the week, then check each day against both
rules and fix any that break them. Show the result as a table with meal, main
ingredient, and cook time. Stop only when all 7 days pass both rules.
```
