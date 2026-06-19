# Test coverage loop

> Drive coverage to the bar with a green suite, not just more test files.

**Goal:** The full test suite passes at 100% coverage (or your team's agreed bar).

- **Trigger:** When coverage has slipped, or before locking a module.
- **Action:** Find uncovered lines, write meaningful tests for them, run the suite.
- **Proof:** The coverage report and a green suite.
- **Memory:** Lines already covered this run, so the agent targets the gaps.
- **Stop condition:** Coverage hits the bar and the suite is green.

## Starter prompt

```
Get this module to [100]% test coverage with a passing suite. Find uncovered lines,
write tests that actually exercise the behavior (not just touch the line), and run
the suite each pass. Show the coverage report after every pass. Do not delete or
weaken existing tests to game coverage. Stop only when coverage hits the bar and the
full suite is green.
```
