# Loop Library

A collection of repeatable AI agent workflows built around one simple idea: give the agent a **goal** and a **loop**, not a one-off request.

Most people use AI like a vending machine. Type a request, get one output, eyeball it, retype it if it is wrong. That works for quick stuff and falls apart the moment a task has more than one round of work in it. Loops fix that.

## The pattern

A **goal** is what "done" looks like, in a sentence you can check.
A **loop** is the agent doing work, checking its own work, then deciding whether to go again.
A **stop condition** is the measurable line that tells the agent when it is allowed to quit.

Every loop in here follows the same five-part shape:

- **Trigger** - when the workflow kicks off
- **Action** - the steps the agent repeats
- **Proof** - how it verifies the work actually meets the bar
- **Memory** - what it carries between rounds so it does not repeat itself
- **Stop condition** - the measurable line that ends the loop

## Good goal vs bad goal

A bad goal is vague, so the agent never knows when to stop. A good goal reads like a finish line.

| Bad | Good |
|-----|------|
| Make the page faster | Every page loads in under 50ms |
| Add some tests | The full test suite passes at 100% coverage |
| Clean up the docs | Documentation matches the current implementation, finished as a reviewable pull request |

If you cannot write the stop condition, you do not have a goal yet, you have a wish. Tighten it until you can.

## The loops

**Everyday**
- [Inbox triage](loops/everyday/inbox-triage.md)
- [Weekly meal plan](loops/everyday/meal-plan.md)
- [Trip itinerary](loops/everyday/trip-itinerary.md)

**UX Research**
- [Interview synthesis](loops/ux-research/interview-synthesis.md)
- [Survey open-text coding](loops/ux-research/survey-open-text.md)
- [Usability findings](loops/ux-research/usability-findings.md)

**Design**
- [Component audit](loops/design/component-audit.md)
- [Accessibility pass](loops/design/accessibility-pass.md)
- [Reference match](loops/design/reference-match.md)

**Engineering**
- [Test coverage](loops/engineering/test-coverage.md)
- [Production error sweep](loops/engineering/production-error-sweep.md)
- [Ticket to PR-ready](loops/engineering/ticket-to-pr-ready.md)
- [Fresh clone](loops/engineering/fresh-clone.md)

## Write your own

Copy [TEMPLATE.md](TEMPLATE.md) and fill in four lines:

1. **Goal** - what does done look like, in a sentence I can check?
2. **Stop condition** - the measurable line. If I cannot tell whether it is met by looking, rewrite it.
3. **Proof** - what does the agent show me to prove the bar is hit?
4. **Memory** - what should it carry between rounds so it does not loop forever or repeat itself?

That is the whole thing. Specific goal, a loop that proves its own work, and a line that says when to stop. The difference between an agent that spins and one that actually finishes.

## Credit

The goal + loop + stop condition framing here is my own take on a pattern that shows up in a lot of agent work. If you want a larger, engineering-heavy set to study, the [Forward Future Loop Library](https://signals.forwardfuture.ai/loop-library/) is worth a read.
