# Feature: Add Card Import/Export

## Summary
Add JSON import/export for decks and cards, preserving deck metadata, category assignments, and scheduling state.

## Why
Local flashcard apps are more useful when users can back up and restore their decks. Import/export also enables sharing decks between users and moving data between devices.

## Acceptance Criteria
- [ ] Add an export action that downloads a JSON file with decks, cards, categories, and scheduler fields.
- [ ] Add an import action that can read the exported JSON format and merge or replace existing data.
- [ ] Preserve `easiness`, `interval`, `repetitions`, and `nextReviewAt` during export/import.
- [ ] Validate the import file and show errors for invalid format.

## Implementation Notes
- Store export format schema in a shared helper file.
- Use file input and `Blob` download for local JSON export/import.
- Consider add-on merge strategy for decks with the same name.
