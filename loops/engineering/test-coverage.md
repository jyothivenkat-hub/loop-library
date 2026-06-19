# Test coverage

> Drive coverage to the bar with a green suite, not just more test files.

## Goal (the what)

- **Objective:** Raise test coverage on a module.
- **Success criteria:** Coverage hits the agreed bar (e.g. 100%) and the full suite passes.
- **Constraints:** Tests must exercise real behavior. Do not delete or weaken tests to game the number.
- **Context:** The module, the test runner, and the coverage tool.

## Loop (the how)

- **Think:** Read the coverage report, pick the next uncovered path.
- **Act:** Write a meaningful test for it.
- **Observe:** Run the suite and the coverage report.
- **Reflect / Plan:** Target the next gap, fix any test that broke.
- **Stop when:** Coverage hits the bar and the suite is green.

## Starter prompt

```
Get this module to [100]% coverage with a passing suite. Read the coverage report,
find uncovered lines, and write tests that actually exercise the behavior, not just
touch the line. Run the suite each pass. Do not delete or weaken existing tests. Show
the coverage report after every pass. Stop only when coverage hits the bar and the
full suite is green.
```
