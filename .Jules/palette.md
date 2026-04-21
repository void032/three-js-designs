## 2026-04-06 - [Accessible character-based animations]
**Learning:** Text-based animations that fragment content into spans (e.g., for staggering effects) can break screen reader clarity as they may read each character individually.
**Action:** Use `aria-label` on the parent interactive element to provide the full text and `aria-hidden="true"` on the individual spans to hide the fragmented characters from assistive technologies.
