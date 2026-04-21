## 2025-03-31 - [Keyboard Animation Consistency]
**Learning:** Animations triggered only on `:hover` exclude keyboard users from the "delightful" parts of the UX. Using `:focus-visible` to trigger the same animations ensures a consistent experience across input methods.
**Action:** Always pair `:hover` animation triggers with `:focus-visible` to maintain parity between mouse and keyboard interactions.
