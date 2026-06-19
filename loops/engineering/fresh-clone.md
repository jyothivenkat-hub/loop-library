# Fresh clone loop

> Prove a new dev can go from clone to running app using only the README.

**Goal:** A clean checkout reaches a running app using only the README.

- **Trigger:** Before onboarding someone, or after changing setup steps.
- **Action:** Clone fresh, follow the README step by step, hit an error, fix the README, start over from clean.
- **Proof:** The app runs on a clean environment with no steps outside the README.
- **Memory:** Steps already verified, so each pass starts where the last gap was found.
- **Stop condition:** A clean environment reaches a running app using only the README.

> Great for catching the setup steps that only live in someone's head.

## Starter prompt

```
Verify our setup docs. Start from a clean clone with nothing pre-installed beyond a
stated baseline. Follow the README exactly, step by step. The moment something fails
or needs a step that is not written down, fix the README, then start over from a
clean clone. Stop only when a clean environment reaches a running app using only the
README, with no undocumented steps.
```
