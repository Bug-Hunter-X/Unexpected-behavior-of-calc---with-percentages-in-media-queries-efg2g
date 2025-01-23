# Unexpected behavior of calc() with percentages in media queries

This repository demonstrates a bug where the CSS `calc()` function produces unexpected results when used with percentages inside media queries.  The issue is particularly noticeable in older browsers or with complex CSS layouts.

## Bug Description
The `calc()` function, when used to calculate a width (or other properties) as a percentage minus a fixed value, behaves incorrectly within a media query. The expected behavior is that the element's width should adjust based on the viewport size and the calculation. However, in some situations, the calculation is inaccurate, leading to unexpected rendering issues.

## Steps to Reproduce
1. Clone this repository.
2. Open `bug.css` and examine the provided CSS code.
3. Open `index.html` (which you would need to create - a simple HTML file with an element having the id `myElement`) in a web browser.
4. Resize the browser window to trigger the media query.
5. Observe that the width of the element (`#myElement`) is not correctly calculated.

## Solution
The solution involves carefully considering how the calculation is structured and potentially using alternative approaches to achieve the desired responsiveness.