## 2025-05-14 - Accessible Split-Text Animations and Keyboard Parity

**Learning:** Fragmentation of text into individual characters (e.g., via `<span>`) for animation purposes degrades screen reader experience by causing them to read character by character. Additionally, focus states are often overlooked in "delightful" animation systems, excluding keyboard users from the experience.

**Action:** Always use `aria-label` on the parent interactive element to provide the full text and `aria-hidden="true"` on the individual character spans. Pair `:hover` with `:focus-visible` for animations and use high-contrast outlines (e.g., `outline: 2px solid #ffffff; outline-offset: 4px;`) for focus indicators.
