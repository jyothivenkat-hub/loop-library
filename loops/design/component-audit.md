# Component audit loop

> Drag every screen back onto the design system, no hardcoded values left.

**Goal:** Every button, input, and card uses a token from the design system, with zero hardcoded colors or spacing.

- **Trigger:** Before a release, or when the UI has drifted off-system.
- **Action:** Scan the screens, flag each off-system value, propose the matching token, apply it.
- **Proof:** A list of violations that shrinks each round, ending at zero.
- **Memory:** Which components are already clean, so re-runs skip them.
- **Stop condition:** Zero hardcoded values remain, every flagged item maps to a token.

## Starter prompt

```
Audit these screens against our design system tokens. Find every hardcoded color,
spacing, radius, or font value on buttons, inputs, and cards. For each, propose the
matching token and apply it. Show the running list of violations and how it shrinks
each pass. Stop only when zero hardcoded values remain and every element maps to a
token. Flag anything that has no matching token so we can add one.
```
