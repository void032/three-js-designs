## 2025-05-14 - Accessibility for Split-Text Animations
**Learning:** Character-wrapping text animations (split-text) cause screen readers to read words character-by-character, creating a poor experience.
**Action:** Always set `aria-label` with the full text on the parent element and `aria-hidden="true"` on the individual character spans.

## 2025-05-14 - Misleading Cursor Feedback
**Learning:** Using `cursor: pointer` on non-interactive elements like headings implies clickability and confuses users.
**Action:** Ensure `cursor: pointer` is only used on truly interactive elements (links, buttons, inputs).
## 2025-05-15 - [Accessible Animated Text]
**Learning:** Text split into spans for animation (e.g., via a `wrapCharacters` function) is often read character-by-character by screen readers, making it unintelligible.
**Action:** Always apply `aria-label` with the full text to the parent element and `aria-hidden="true"` to the individual character spans. Pair this with `:focus-visible` styles to ensure keyboard accessibility matches hover effects.
