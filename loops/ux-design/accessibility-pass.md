# Accessibility pass

> Hit WCAG AA contrast and visible focus on every screen, with the numbers to prove it.

## Goal (the what)

- **Objective:** Make every screen meet a baseline accessibility bar.
- **Success criteria:** All screens pass WCAG AA contrast and every interactive element has a visible focus state.
- **Constraints:** Keep the brand palette where possible, adjust only what fails.
- **Context:** The screens, the palette, and the WCAG AA thresholds.

## Loop (the how)

- **Think:** Pick a screen, check text and UI contrast and focus states.
- **Act:** Fix failing contrast and add missing focus states.
- **Observe:** Re-measure the contrast ratios and confirm focus states render.
- **Reflect / Plan:** Record before and after values, move to the next screen.
- **Stop when:** Every screen passes AA contrast and every control has a visible focus state.

## Starter prompt

```
Run an accessibility pass on these screens. For each, check text and UI contrast
against WCAG AA and confirm every interactive element has a visible focus state. Fix
failures and re-check. Report before and after contrast ratios for anything you
changed, and list each control with its focus state. Stop only when every screen
passes AA contrast and every control has a visible focus state.
```
