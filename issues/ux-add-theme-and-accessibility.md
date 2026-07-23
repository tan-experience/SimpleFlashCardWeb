# UX Enhancement: Add Theme and Accessibility Support

## Summary
Add a dark/light theme toggle and improve accessibility with better contrast, focus outlines, and screen-reader labels.

## Why
A theme toggle helps users study in different lighting conditions, while accessibility improvements make the app usable for more people.

## Acceptance Criteria
- [ ] Add a dark/light theme toggle in the header or settings area.
- [ ] Apply consistent high-contrast styling for buttons and form fields.
- [ ] Add ARIA labels for important controls and ensure focus states are visible.
- [ ] Save the chosen theme in local storage.

## Implementation Notes
- Use CSS custom properties to define theme colors.
- Add a `theme` state in `App.tsx` or a shared context.
- Use semantic HTML and accessible button labels in `Deck`, `Study`, and `CardEditor` pages.
