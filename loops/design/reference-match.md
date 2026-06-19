# Reference match loop

> Make the build match the mock on every axis you name, not just "looks close."

**Goal:** The built screen matches the design mock across spacing, type scale, color, and layout.

- **Trigger:** After a screen is built from a design.
- **Action:** Compare build to mock, list every difference per axis, fix, compare again.
- **Proof:** A diff list per axis that shrinks to zero.
- **Memory:** Axes already matching, so re-runs check only what is left.
- **Stop condition:** The build matches the reference across every measured axis.

> "Looks good" is the worst possible stop condition. Name the axes (spacing, type scale, color, layout) and the agent has something to check against.

## Starter prompt

```
Compare this built screen to the design mock across four axes: spacing, type scale,
color, and layout. List every difference under each axis. Fix them, then compare
again. Keep looping until each axis has zero differences. Show the remaining diff
list after every pass. Stop only when the build matches the mock on all four axes.
```
