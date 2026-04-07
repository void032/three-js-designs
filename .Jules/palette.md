## 2026-04-07 - Staggered text animations and accessibility
**Learning:** Fragmenting text into individual spans for animation causes screen readers to read words character-by-character. Additionally, these animations are often only triggered on `:hover`, excluding keyboard users.
**Action:** Use `aria-label` on the parent interactive element and `aria-hidden="true"` on the individual character spans. Always pair `:hover` triggers with `:focus-visible` in CSS.

## 2026-04-07 - Misleading Interactivity
**Learning:** Using `cursor: pointer` on non-interactive elements like headings can confuse users by falsely implying clickability.
**Action:** Only use `cursor: pointer` for genuinely interactive elements (links, buttons, etc.) and remove it from purely decorative or informative elements.
