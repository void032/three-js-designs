## 2025-05-14 - Accessible Text Animations
**Learning:** For text-based animations that fragment content (e.g., wrapping characters in spans), use `aria-label` on the parent interactive element and `aria-hidden="true"` on the individual spans to preserve screen reader clarity.
**Action:** Always pair character-level animations with a full-string `aria-label` and hide the animated fragments from screen readers.

## 2025-05-14 - Semantic Navigation and Keyboard Focus
**Learning:** Simple changes like converting a `div` to a `<nav>` element and adding `:focus-visible` styles significantly improve accessibility for assistive technologies and keyboard users with minimal code changes.
**Action:** Prioritize semantic HTML tags and ensure visible focus states for all interactive elements.
