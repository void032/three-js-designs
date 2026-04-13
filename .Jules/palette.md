## 2026-04-13 - [Text Fragmentation Accessibility]
**Learning:** Animated text that is fragmented into individual spans for character-based effects (like the wrapCharacters function) is read letter-by-letter by screen readers, creating a poor experience.
**Action:** Always apply aria-label to the parent element containing the full text and aria-hidden="true" to the individual character spans to ensure screen reader clarity while maintaining visual effects.
