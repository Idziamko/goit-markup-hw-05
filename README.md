GoIT Markup Homework #5: Modal Window and Forms
Description of the Assignment
This repository contains the solution for GoIT Markup Homework #5. The main goal of this assignment is to add interactive UI elements: a feedback modal window and a newsletter subscription form in the footer, using advanced CSS positioning and form styling techniques.

The work focuses on ensuring semantic correctness, accessibility (hidden checkbox, label binding), and implementing smooth CSS transitions.

🛠️ Key Technical Features
The following key technical solutions were implemented in this assignment:

1. Modal Window Mechanism
   Backdrop Implementation: A fixed .model-overlay was created, which fills 100% of the viewport and uses a high z-index to overlap the content.

Centering: The modal window (.model) is centered within the backdrop using Flexbox (justify-content: center, align-items: center on .model-overlay).

Toggle Mechanism: A toggle class .is-open is used to show/hide the modal window and enable interactivity (opacity: 1, pointer-events: auto).

2. Form Styling and Interactivity
   Forms: Two forms were created: a contact form in the modal window and a subscription form in the footer.

Icon Positioning: Icons inside input fields are positioned using absolute positioning (position: absolute) relative to their parent element.

Focus Effects: When an input receives focus, its border and icon change to an accent color (#4d5ae5).

3. Custom Checkbox
   Accessibility: The original checkbox is hidden using the .visually-hidden class.

Custom Styling: A visual representation (a 16x16px square) was created with an SVG checkmark from a sprite, which appears in the :checked state.

4. Semantics and Accessibility
   Labels: All input fields (including textarea) are linked to their corresponding text descriptions using the <label> tag with a for/id connection.

Buttons: The type="submit" attribute is set for the submission buttons.

5. CSS Transitions
   Smooth Effects: Smooth transitions are configured for all interactive elements (buttons, links, inputs, modal window) with a duration of 250ms and the cubic-bezier(0.4, 0, 0.2, 1) timing function.

🚀 Live Page
The project is hosted on GitHub Pages. You can view the live result here:

[https://idziamko.github.io/goit-markup-hw-05/]
