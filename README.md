# AI Agent Goal & Loop Library

Ready-to-use goals and loop patterns that turn AI from a fancy chatbot into an autonomous worker.

Most people give AI one prompt and hope for the best. Agents with a clear **goal** and a robust **loop** are different: they handle multi-step work, recover from failures, use tools, and iterate until the work is actually done.

## Goal vs Loop

A **Goal** is the destination, the clear objective you want the agent to achieve. It defines what success looks like.

A **Loop** (the Agent Loop or Reasoning Loop) is the engine, the repeating cycle the agent runs to get there: think, act, observe, adjust, repeat until the goal is met or it runs out of steps.

- **Goal = the "What"**
- **Loop = the "How"**

## The components

**Goal components** (usually defined once):

- Clear objective
- Success criteria
- Constraints (budget, time, format)
- Context (background information)

**Loop components** (the repeating cycle):

- **Think** - reason about the current state and the next best step
- **Act** - use a tool, write code, send an email
- **Observe** - read the result of the action
- **Reflect / Plan** - update understanding, decide the next move
- **Repeat** - until the goal is achieved or a stopping condition is met

## Good goal vs bad goal

A bad goal is vague, so the agent never knows when to stop.

> "Help me with my product."

A good goal is specific, has success criteria, and reads like a finish line.

> "Conduct a competitive analysis of 5 similar productivity tools, identify 3 key UX gaps in our current app, and deliver a prioritized list of 8 improvement recommendations with Figma mockup concepts."

If you cannot tell whether the result meets the goal by looking at it, tighten the goal until you can.

## The library

Each file has a Goal (objective, success criteria, constraints, context), a Loop config (think, act, observe, reflect, stop), and a starter prompt you can paste straight into an agent.

**Everyday**
- [Weekly planning](loops/everyday/weekly-plan.md)
- [Inbox triage](loops/everyday/inbox-triage.md)
- [Meal plan](loops/everyday/meal-plan.md)
- [Trip itinerary](loops/everyday/trip-itinerary.md)

**UX Research**
- [Interview synthesis](loops/ux-research/interview-synthesis.md)
- [Survey open-text coding](loops/ux-research/survey-open-text.md)
- [Usability findings](loops/ux-research/usability-findings.md)

**UX Design**
- [Checkout redesign](loops/ux-design/checkout-redesign.md)
- [Component audit](loops/ux-design/component-audit.md)
- [Accessibility pass](loops/ux-design/accessibility-pass.md)
- [Reference match](loops/ux-design/reference-match.md)

**Engineering**
- [FastAPI backend](loops/engineering/fastapi-backend.md)
- [Test coverage](loops/engineering/test-coverage.md)
- [Production error sweep](loops/engineering/production-error-sweep.md)
- [Ticket to PR-ready](loops/engineering/ticket-to-pr-ready.md)
- [Fresh clone](loops/engineering/fresh-clone.md)

**Product**
- [Go-to-market strategy](loops/product/gtm-strategy.md)
- [Competitive analysis](loops/product/competitive-analysis.md)

## Write your own

Copy [TEMPLATE.md](TEMPLATE.md). Write the goal first (objective, success criteria, constraints, context), then the loop (think, act, observe, reflect, stop). Writing good goals: be specific, include success criteria, add context and constraints, use action verbs. Designing loops: give the agent good tools and memory, add reflection steps, set clear stopping conditions.

Mastering goals gives you direction. Mastering loops gives you execution power. Combine both and you turn AI from a helpful assistant into a true collaborator.

---

*For a larger, engineering-heavy set to study, the [Forward Future Loop Library](https://signals.forwardfuture.ai/loop-library/) is worth a read.*
