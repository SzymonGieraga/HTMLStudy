# HTML/CSS Recruitment Study

This repository contains my solution for  recruitment task. The goal was to create a fully responsive webpage using **only HTML and CSS**, without the use of JavaScript, external frameworks, or image files.

## Project Overview

### Screen Breakpoints & Layout

The layout adapts to three main viewports to ensure all elements remain visible without scrolling:

1.  **Desktop View (> 900px)**
    * **Layout:** Horizontal alignment.
    * **Side Panel:** White background, positioned on the right side.
    * **Background:** Green.

2.  **Tablet View (583px - 900px)**
    * **Layout:** Middle elements shift position relative to the diamonds.
    * **Side Panel:** Background color changes to **Red** (`#C83737`).
    * **Alignment:** Elements adjust to fit narrower screens while maintaining a row-based structure where possible.

3.  **Mobile View (< 583px)**
    * **Layout:** Vertical (Column) alignment. All elements stack vertically.
    * **Side Panel:** Background color changes to **Blue** (`#0000ff`). The panel resizes and moves to the bottom of the flow.

## Technical Implementation

### CSS-Only Animations 

**How it works:**
1.  **State Management:** Hidden `<input type="radio">` elements track the state of the interactive components (State A vs. State B).
2.  **Triggers:** The visible elements (Diamonds, Side Panel) are wrapped in or paired with `<label>` tags linked to these inputs.
3.  **Execution:** When a user clicks an element, the corresponding radio input is checked. CSS selectors (like `input:checked ~ .target`) then apply specific `@keyframes` animations or transitions.
4.  **Looping:** By alternating between two radio inputs, the user can click the element repeatedly to re-trigger the animation effect.

### Animations
* **Diamonds:** Clicking a diamond rotates it 360 degrees. First click rotates the diamond to the left, second to the right.
* **Side Panel:** Clicking the panel triggers a text color cycle animation (Black → White → Black).

## How to Run

Simply download the repository and open `index.html` in any modern web browser.

### What is the `plan.txt`?

It's an under 1000 characters room makeover plan written in English (needed for the recruitment).