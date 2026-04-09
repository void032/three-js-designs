## 2026-04-09 - Accessibility for Animated Text
**Learning:** Fragmenting text into spans for animation (e.g., character-by-character hover effects) breaks screen reader accessibility by causing them to read character-by-character.
**Action:** Always add `aria-label` to the parent element with the full text and `aria-hidden="true"` to the individual spans.

## 2026-04-09 - Focus Visibility in Dark Themes
**Learning:** Default focus rings are often invisible on dark, high-contrast backgrounds like this space theme.
**Action:** Implement custom `:focus-visible` styles using `outline: 2px solid #ffffff;` with an `outline-offset: 4px;` to ensure visibility.

## 2026-04-09 - Meaningful Cursors
**Learning:** `cursor: pointer` on non-interactive elements (like `h1`) creates false affordance, leading users to expect an interaction that doesn't exist.
**Action:** Only use `cursor: pointer` for elements with defined click or tap behaviors.
