# Feature: Add Study Scope Selector

## Summary
Add the ability to choose which cards to study by scope: single deck, category, or all due cards across decks.

## Why
The current app only supports studying a single deck at a time. A study scope selector will let users review all due cards or study across multiple decks, which is more flexible and better reflects real learning habits.

## Acceptance Criteria
- [ ] Add a scope selector on the study start screen.
- [ ] Support at least these options: current deck, all due cards, due cards in selected category.
- [ ] Load the correct set of cards for a session based on the selected scope.
- [ ] Persist the most recent scope choice for the current session.

## Implementation Notes
- Add scope metadata to the study session state.
- Use existing scheduler logic to filter cards by `nextReviewAt` and deck/category membership.
- Extend route handling if needed to support `/study/:scope/:id`.
