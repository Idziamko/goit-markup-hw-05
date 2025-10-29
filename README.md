# GoIT Markup Homework #5: Modal Window and Forms

## Description of the Assignment

This repository contains the solution for GoIT Markup Homework #5. The main goal of this assignment is to add interactive UI elements: a feedback modal window and a newsletter subscription form in the footer, using advanced CSS positioning and form styling techniques.

The work focuses on ensuring semantic correctness, accessibility (hidden checkbox, label binding), and implementing smooth CSS transitions.

---

## 🛠️ Key Technical Features

The following key technical solutions were implemented in this assignment:

### Modal Window Mechanism
* **Backdrop Implementation:** A fixed `.model-overlay` (или `.backdrop`) was created, which fills 100% of the viewport and uses a high `z-index` to overlap the content.
* **Centering:** The modal window (`.model`) is centered within the backdrop using `position: absolute` with `top: 50%`, `left: 50%`, and `transform: translate(-50%, -50%)`.
* **Toggle Mechanism:** A toggle class (`.is-open`) is used to show/hide the modal window. This class typically changes `visibility` and `opacity` to control the modal's appearance and `transform` for the animation.

### Form Styling and Interactivity
* **Forms:** Two forms were created: a contact form in the modal window and a subscription form in the footer.
* **Icon Positioning:** Icons inside input fields are positioned using `position: absolute` relative to their parent container (e.g., `left: 16px`, `top: 50%`, `transform: translateY(-50%)`).
* **Focus Effects:** When an input receives focus, its `border-color` and the `fill` color of its associated icon change to the accent color (`#4d5ae5`).

### Custom Checkbox
* **Accessibility:** The original `<input type="checkbox">` is hidden using the `.visually-hidden` class.
* **Custom Styling:** A visual representation (a `<span>` acting as a 16x16px square) was created with an SVG checkmark from a sprite, which appears (by changing `background-color` and icon `fill`) when the input is in the `:checked` state.

### Semantics and Accessibility
* **Labels:** All input fields (including `<textarea>`) are linked to their corresponding text descriptions using the `<label>` tag with a matching `for`/`id` connection.
* **Buttons:** The `type="submit"` attribute is set for the submission buttons.

### CSS Transitions
* **Smooth Effects:** Smooth transitions are configured for all interactive elements (buttons, links, inputs, modal window) with a duration of `250ms` and the `cubic-bezier(0.4, 0, 0.2, 1)` timing function.
* **Property-Specific:** Transitions are applied to specific properties like `border-color`, `fill`, and `background-color`, not just `all`.

---

## 🚀 Live Page

The project is hosted on GitHub Pages. You can view the live result here:

**[https://idziamko.github.io/goit-markup-hw-05/]**
