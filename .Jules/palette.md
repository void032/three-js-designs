## 2026-04-19 - [Accessibility of Fragmented Text Animations]
**Learning:** Text-based animations that split words into individual character spans (like the `wrapCharacters` function in this repo) cause screen readers to read words letter-by-letter, breaking the user experience.
**Action:** Always set `aria-label` with the full text on the parent element and apply `aria-hidden="true"` to the individual character spans. Pair these animations with `:focus-visible` states to ensure keyboard users have equal visual feedback to hover users.
