# Ticket to PR-ready

> Take a bug ticket all the way to a reviewable PR, with a regression test.

## Goal (the what)

- **Objective:** Fix the bug in a ticket and get it review-ready.
- **Success criteria:** The bug is fixed and verified, a regression test passes, and the PR is open.
- **Constraints:** Add a regression test that fails on the old code. Do not change unrelated behavior.
- **Context:** The ticket, the repo, and how to run the suite.

## Loop (the how)

- **Think:** Reproduce the bug, form a hypothesis about the cause.
- **Act:** Apply a fix and add a regression test.
- **Observe:** Run the test and the suite, confirm the bug no longer reproduces.
- **Reflect / Plan:** If it still fails, revise the fix; note dead ends so they are not retried.
- **Stop when:** The bug no longer reproduces, the regression test passes, the suite is green, and the PR is open.

## Starter prompt

```
Take this ticket to a review-ready PR. First reproduce the bug and confirm you can
trigger it. Then fix it. Add a regression test that fails on the old code and passes
on the fix. Run the full suite. Open a PR describing the root cause and the fix. Stop
only when the bug no longer reproduces, the regression test passes, the suite is
green, and the PR is open.
```
