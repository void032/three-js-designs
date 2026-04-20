## 2026-04-20 - [Accessibility and Keyboard Parity for Fragmented Text Animations]
**Learning:** Fragmenting text into individual spans for animations (like in `wrapCharacters`) breaks screen reader accessibility by reading characters individually. It also often leaves keyboard users without visual feedback if animations only trigger on `:hover`.
**Action:** Use `aria-label` on the parent and `aria-hidden="true"` on the character spans. Ensure all `:hover` animation triggers also include `:focus-visible` to maintain keyboard parity.
