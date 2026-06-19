# Accessibility pass loop

> Hit WCAG AA contrast and visible focus on every screen, with the numbers to prove it.

**Goal:** Every screen meets WCAG AA contrast and every interactive element has a visible focus state.

- **Trigger:** Before shipping, or as part of a quality pass.
- **Action:** Check each screen's contrast ratios and focus states, fix failures, re-check.
- **Proof:** Before and after contrast values per element, and a confirmed focus state for each control.
- **Memory:** Screens already passing, so re-runs focus on the rest.
- **Stop condition:** All screens pass AA contrast, every control has a visible focus state.

## Starter prompt

```
Run an accessibility pass on these screens. For each, check text and UI contrast
against WCAG AA, and confirm every interactive element has a visible focus state.
Fix failures and re-check. Report before and after contrast ratios for anything you
changed, and list each control with its focus state. Stop only when every screen
passes AA contrast and every control has a visible focus state.
```
