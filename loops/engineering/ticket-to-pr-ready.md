# Ticket to PR-ready loop

> Take a bug ticket all the way to a reviewable PR, with a regression test.

**Goal:** The failure described in the ticket is fixed, verified, and ready for review.

- **Trigger:** A bug ticket lands.
- **Action:** Reproduce the bug, fix it, add a regression test, run the suite, open the PR.
- **Proof:** The bug reproduces before the fix and cannot be reproduced after, and the regression test passes.
- **Memory:** What was already tried, so dead ends are not repeated.
- **Stop condition:** The bug is reproduced then cannot be reproduced, the regression test passes, the PR is open.

## Starter prompt

```
Take this ticket to a review-ready PR. First reproduce the bug and confirm you can
trigger it. Then fix it. Add a regression test that fails on the old code and passes
on the fix. Run the full suite. Open a PR with a description of the root cause and
the fix. Stop only when the bug no longer reproduces, the regression test passes,
the suite is green, and the PR is open.
```
