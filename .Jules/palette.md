## 2026-04-02 - Fragmented Text Accessibility
**Learning:** Animating text by wrapping individual characters in `<span>` tags causes screen readers to announce the word letter-by-letter, breaking the user experience for visually impaired users.
**Action:** Always set an `aria-label` with the full text on the parent interactive element and add `aria-hidden="true"` to the individual character spans to ensure the word is read correctly as a single unit.
