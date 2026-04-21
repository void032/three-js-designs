## 2025-05-15 - [Accessible Animated Text]
**Learning:** Text split into spans for animation (e.g., via a `wrapCharacters` function) is often read character-by-character by screen readers, making it unintelligible.
**Action:** Always apply `aria-label` with the full text to the parent element and `aria-hidden="true"` to the individual character spans. Pair this with `:focus-visible` styles to ensure keyboard accessibility matches hover effects.
