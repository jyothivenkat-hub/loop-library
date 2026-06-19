# Usability findings loop

> Every task failure logged with severity and a fix, nothing left as "needs a look."

**Goal:** Every task failure in the session recordings is logged with severity, the step it happened on, and a suggested fix.

- **Trigger:** After usability sessions are recorded.
- **Action:** Review each session, mark each task failure, record severity, the step, and a fix.
- **Proof:** A findings log with one row per failure, fully filled in.
- **Memory:** Failures already logged, so duplicates across sessions get merged with a count.
- **Stop condition:** Every recorded session reviewed, every failure has severity and a fix, nothing left as "needs a look."

## Starter prompt

```
Here are notes or recordings from [N] usability sessions, plus the task list. For
each session, find every task failure or struggle. Log each one with: the task, the
step it happened on, a severity (critical, major, minor), and a suggested fix. Merge
the same failure across sessions into one row with a participant count. Stop when
every session is reviewed and every logged failure has a severity and a fix, with
nothing marked "needs a look."
```
