## 2025-05-14 - Accessibility for Split-Text Animations
**Learning:** Character-wrapping text animations (split-text) cause screen readers to read words character-by-character, creating a poor experience.
**Action:** Always set `aria-label` with the full text on the parent element and `aria-hidden="true"` on the individual character spans.

## 2025-05-14 - Misleading Cursor Feedback
**Learning:** Using `cursor: pointer` on non-interactive elements like headings implies clickability and confuses users.
**Action:** Ensure `cursor: pointer` is only used on truly interactive elements (links, buttons, inputs).
