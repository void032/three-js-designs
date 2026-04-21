## 2026-04-20 - [Accessibility and Keyboard Parity for Fragmented Text Animations]
**Learning:** Fragmenting text into individual spans for animations (like in `wrapCharacters`) breaks screen reader accessibility by reading characters individually. It also often leaves keyboard users without visual feedback if animations only trigger on `:hover`.
**Action:** Use `aria-label` on the parent and `aria-hidden="true"` on the character spans. Ensure all `:hover` animation triggers also include `:focus-visible` to maintain keyboard parity.
## 2025-05-14 - [Dynamic Staggered Animation & Keyboard Accessibility]
**Learning:** Hardcoding staggered animations with CSS `nth-child` is fragile and limits the effect to a specific character count. Moving this logic to JavaScript using inline `animation-delay` ensures the UX enhancement works for text of any length while keeping the code maintainable. Additionally, adding `:focus-visible` styles is a non-intrusive way to provide necessary visual feedback for keyboard users.
**Action:** Use JS for character-based staggered animations in dynamic text and always pair navigation elements with `:focus-visible` states.
## 2026-04-08 - Improving Screen Reader Support for Character-Wrapped Animations
**Learning:** Fragmenting text into spans for animations (like staggered letter entry) causes screen readers to read the text character-by-character, which is a poor user experience.
**Action:** Always add `aria-label` with the full text to the parent element and set `aria-hidden="true"` on the individual spans to ensure the word is read correctly by assistive technology while maintaining the visual effect.

## 2026-04-08 - Visual Feedback for Interactive vs. Non-interactive Elements
**Learning:** Using `cursor: pointer` on non-interactive elements like headings can mislead users into thinking they are clickable, especially in minimalist designs.
**Action:** Reserved `cursor: pointer` for truly interactive elements (links, buttons) and ensured non-interactive headings use the default cursor.

