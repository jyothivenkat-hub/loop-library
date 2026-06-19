# Inbox triage loop

> Get to a clean inbox with a decision logged for every message.

**Goal:** Every email from the last 24 hours is either archived, replied to, or flagged with a reason.

- **Trigger:** Once a day, or whenever unread count gets uncomfortable.
- **Action:** Read each unread email, decide the category (archive, reply, flag), take the action.
- **Proof:** No unread email remains without a logged decision.
- **Memory:** Which senders or threads are already handled, so re-runs do not redo them.
- **Stop condition:** Inbox zero for the last 24 hours, with a short summary of what was flagged and why.

## Starter prompt

```
Go through my unread emails from the last 24 hours. For each one, decide: archive,
reply, or flag. Draft replies for anything that needs one. Flag anything that needs
my decision with a one-line reason. Keep going until every email has a decision.
Then show me a summary: how many archived, the drafts you wrote, and the flagged
list with reasons. Stop when nothing from the last 24 hours is left undecided.
```
