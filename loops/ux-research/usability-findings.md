# Usability findings

> Every task failure logged with severity and a fix, nothing left as "needs a look."

## Goal (the what)

- **Objective:** Log usability problems from session recordings.
- **Success criteria:** Every task failure has a severity, the step it happened on, and a suggested fix.
- **Constraints:** Merge the same failure across sessions into one entry with a participant count.
- **Context:** The session recordings or notes, and the task list participants attempted.

## Loop (the how)

- **Think:** Review a session, spot where a task failed or the user struggled.
- **Act:** Log the failure with task, step, severity, and a suggested fix.
- **Observe:** Check whether this failure already exists in the log.
- **Reflect / Plan:** Merge duplicates with a count, move to the next session.
- **Stop when:** Every session is reviewed and every logged failure has a severity and a fix.

## Starter prompt

```
Here are notes or recordings from [N] usability sessions, plus the task list. For
each session, find every task failure or struggle. Log each with the task, the step
it happened on, a severity (critical, major, minor), and a suggested fix. Merge the
same failure across sessions into one entry with a participant count. Stop when every
session is reviewed and every logged failure has a severity and a fix, with nothing
marked "needs a look."
```
