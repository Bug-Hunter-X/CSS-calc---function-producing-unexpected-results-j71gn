# CSS calc() Function Unexpected Results

This repository demonstrates a common issue encountered when using the CSS `calc()` function: unexpected results due to unit inconsistencies or complex calculations.  The `bug.css` file contains the erroneous code, while `bugSolution.css` provides a corrected version.

The issue stems from the way `calc()` handles different units and the order of operations.  Care must be taken to ensure that units are consistent and that the expression is correctly structured.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` (you'll need to create a simple HTML file that includes the CSS file) in your browser.
3. Observe the unexpected results.
4. Replace `bug.css` with `bugSolution.css` to see the corrected behavior.

## Solution
The solution often involves:
* Ensuring that all units within the `calc()` expression are consistent (e.g., all pixels, or all percentages).
* Using parentheses to control the order of operations within complex calculations.
* Carefully inspecting the parent element's dimensions and any potential margins or padding that could affect the calculation.