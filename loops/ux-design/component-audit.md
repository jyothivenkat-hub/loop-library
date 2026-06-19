# Component audit

> Drag every screen back onto the design system, no hardcoded values left.

## Goal (the what)

- **Objective:** Bring the UI back onto the design system.
- **Success criteria:** Every button, input, and card uses a token, with zero hardcoded colors or spacing.
- **Constraints:** Do not change layout or behavior, only swap off-system values for tokens.
- **Context:** The screens and the design system token set.

## Loop (the how)

- **Think:** Scan a screen, find an off-system color, spacing, radius, or font value.
- **Act:** Map it to the matching token and apply it.
- **Observe:** Track the running list of remaining violations.
- **Reflect / Plan:** Flag any value with no matching token, move to the next component.
- **Stop when:** Zero hardcoded values remain and every element maps to a token.

## Starter prompt

```
Audit these screens against our design system tokens. Find every hardcoded color,
spacing, radius, or font on buttons, inputs, and cards. For each, apply the matching
token without changing layout or behavior. Show the violation list shrinking each
pass. Flag anything with no matching token. Stop only when zero hardcoded values
remain and every element maps to a token.
```
