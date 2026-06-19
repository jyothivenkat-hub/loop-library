# Production error sweep

> Clear actionable production errors and confirm they are actually gone.

## Goal (the what)

- **Objective:** Reduce production errors.
- **Success criteria:** Every actionable error is fixed and verified gone in the logs.
- **Constraints:** Do not suppress errors to hide them. Mark non-actionable noise with a reason.
- **Context:** The error log or monitoring tool, and deploy access.

## Loop (the how)

- **Think:** Pull the log, group errors by root cause, rank by impact.
- **Act:** Fix the top actionable cause and deploy.
- **Observe:** Watch the log to confirm the error stops appearing.
- **Reflect / Plan:** Mark non-actionable causes with a reason, move to the next.
- **Stop when:** Every actionable error is fixed and confirmed gone.

## Starter prompt

```
Pull the production error log. Group errors by root cause and rank by impact. For each
actionable cause, find the fix, apply it, and after it ships confirm the error is gone
from the logs. Do not suppress errors. Mark anything non-actionable (noise, third-
party, expected) with a reason so we do not revisit it. Stop only when every actionable
error is fixed and verified gone.
```
