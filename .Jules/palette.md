## 2024-05-15 - Accessible Character-Wrapped Animations
**Learning:** Animations that wrap text into individual `<span>` elements (like for staggered transitions) can break screen reader experiences by announcing characters individually.
**Action:** Use `aria-label` on the parent container to provide the full text and `aria-hidden="true"` on each individual `<span>` to hide the fragmented characters from assistive technologies. Ensure hover-based animations are also triggered by `:focus-visible` for keyboard users.
