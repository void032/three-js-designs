## 2026-04-08 - Improving Screen Reader Support for Character-Wrapped Animations
**Learning:** Fragmenting text into spans for animations (like staggered letter entry) causes screen readers to read the text character-by-character, which is a poor user experience.
**Action:** Always add `aria-label` with the full text to the parent element and set `aria-hidden="true"` on the individual spans to ensure the word is read correctly by assistive technology while maintaining the visual effect.

## 2026-04-08 - Visual Feedback for Interactive vs. Non-interactive Elements
**Learning:** Using `cursor: pointer` on non-interactive elements like headings can mislead users into thinking they are clickable, especially in minimalist designs.
**Action:** Reserved `cursor: pointer` for truly interactive elements (links, buttons) and ensured non-interactive headings use the default cursor.
