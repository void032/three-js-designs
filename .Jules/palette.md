## 2025-05-14 - [Accessible Text Fragmenting]
**Learning:** Text-fragmenting animations (wrapping characters in <span> for staggered effects) cause screen readers to read text letter-by-letter, breaking the user experience.
**Action:** Always pair character-level animations with `aria-label` on the parent container and `aria-hidden="true"` on the individual character spans.
