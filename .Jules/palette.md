## 2025-04-14 - Accessible Character-Split Animations
**Learning:** Text-splitting animations for hover effects (like character staggering) can break screen reader announcements by splitting words into individual characters, and they often exclude keyboard users by only triggering on hover.
**Action:** Always pair character-split animations with an `aria-label` on the parent interactive element and `aria-hidden="true"` on the individual character spans. Additionally, always mirror `:hover` animation triggers with `:focus-visible` to ensure keyboard accessibility.
