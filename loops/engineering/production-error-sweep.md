# Production error sweep loop

> Clear actionable production errors and confirm they are actually gone.

**Goal:** Actionable production errors are fixed and verified gone in the logs.

- **Trigger:** On a schedule, or when the error rate spikes.
- **Action:** Pull the error log, group by root cause, fix the top cause, deploy, watch.
- **Proof:** The error disappears from the logs after the fix ships.
- **Memory:** Which errors are already handled and which were ruled non-actionable, so they are not re-opened.
- **Stop condition:** Every actionable error is fixed and confirmed gone in the logs.

## Starter prompt

```
Pull the production error log. Group errors by root cause and rank by impact. For
each actionable cause, find the fix, apply it, and after it ships confirm the error
is gone from the logs. Mark anything non-actionable (noise, third-party, expected)
with a reason so we do not revisit it. Stop only when every actionable error is
fixed and verified gone.
```
