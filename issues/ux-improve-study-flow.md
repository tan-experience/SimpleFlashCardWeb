# UX Enhancement: Improve Study Flow

## Summary
Refine the study session interface to make card review easier and faster with a clearer reveal flow and keyboard support.

## Why
A smoother study flow improves focus and reduces friction while learning. Clear reveal and rating controls help users stay in the study zone.

## Acceptance Criteria
- [ ] Add a clear reveal button for the card back.
- [ ] Show a progress indicator like "Card 3 of 12".
- [ ] Add keyboard shortcuts for reveal and rating (e.g. `Space` to reveal, `1-5` to rate).
- [ ] Keep the next action button visible after rating so users can continue seamlessly.

## Implementation Notes
- Update study UI in `Study.tsx` to separate reveal and rating states.
- Keep keyboard handlers scoped to the study page.
- Use visual feedback for the selected rating and next card transition.
