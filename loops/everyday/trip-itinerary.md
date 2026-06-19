# Trip itinerary loop

> A day-by-day plan where the logistics actually work, not a wish list of places.

**Goal:** A 3 day itinerary where every stop is within a 15 minute walk of the next and nothing is closed on the day you visit.

- **Trigger:** Planning a short trip.
- **Action:** Draft the days, then check each stop's hours against the visit day and the walking distance to the next stop.
- **Proof:** Each entry shows confirmed hours and walking distance to the following stop.
- **Memory:** Stops already placed, so the agent fills gaps instead of restarting.
- **Stop condition:** Every entry has hours confirmed and walking distance noted, with no gap over 15 minutes.

## Starter prompt

```
Plan a 3 day itinerary for [city]. Rules: each stop must be within a 15 minute walk
of the next, and nothing can be closed on the day I visit it. Draft the days, then
verify each stop's opening hours for that day and the walking distance to the next
stop. Fix anything that breaks a rule. Show hours and walking distance for every
entry. Stop only when all three days pass both rules.
```
