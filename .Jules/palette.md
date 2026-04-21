## 2025-05-14 - Accessible Text Fragmentation Animations
**Learning:** Fragmenting text into spans for animation (e.g., character-by-character hover effects) causes screen readers to announce the text character-by-character, which is a major accessibility barrier.
**Action:** Always add `aria-label` with the full text to the parent element and `aria-hidden="true"` to the individual character spans. Also, ensure animations are triggered by `:focus-visible` to maintain keyboard parity with `:hover`.

## 2025-05-14 - Misleading Cursors on Static Elements
**Learning:** Using `cursor: pointer` on non-interactive elements (like headings) falsely implies they are clickable, leading to user confusion and poor UX.
**Action:** Reserve `cursor: pointer` only for elements with associated click actions or navigation. Use default cursors for static information.
