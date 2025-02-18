# CSS Specificity Bug: Unexpected Font Size Inheritance

This repository demonstrates a common CSS bug related to inheritance and specificity.  The bug arises from unexpected font size behavior due to conflicting style declarations.

## Bug Description

When a `<p>` element is nested within a `<div>`, the font size is unexpectedly smaller than expected. This is because of the specificity of the selectors involved. The `div p` selector overrides the `p` selector, resulting in an unexpected font size.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` to see the buggy CSS code.
3. Open `bugSolution.css` to see the solution.
4. Create an HTML file and test the CSS rules.

## Solution

The solution involves understanding CSS specificity and adjusting the selectors to ensure the intended font size is applied. This might involve using `!important`, though this should be avoided if possible, or restructuring the CSS rules using more specific or less specific selectors.  The solution is demonstrated in `bugSolution.css`

This example highlights the importance of understanding CSS specificity when writing stylesheets to avoid unexpected behavior.