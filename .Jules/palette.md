## 2026-04-12 - Accessible Character Animations
**Learning:** Animating text by wrapping characters in `<span>` tags (e.g., for staggered reveal effects) causes screen readers to announce individual letters instead of full words, severely impacting accessibility.
**Action:** Always apply `aria-label` with the original text to the parent container and `aria-hidden="true"` to the generated `<span>` elements to ensure a coherent screen reader experience while maintaining visual delight.
