# Unexpected Behavior of calc() in linear-gradient with Percentages

This repository demonstrates an unexpected behavior of the `calc()` function in CSS when used with percentages inside a `linear-gradient()` function.  The issue involves calculating a percentage offset within the gradient's color stops.

## Bug Description

The `calc()` function, when used to calculate the position of a color stop in a linear gradient using percentages, doesn't seem to respect the intended calculation.  This leads to the color stops being positioned incorrectly.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` to see the code causing the problem.
3. Open the HTML file (or create your own) and apply the CSS class to an element.  Observe the rendering.
4. Compare it to the expected output in `bugSolution.css` and the corresponding explanation. 

## Solution

The solution involves a workaround.  Instead of using `calc()` with percentages directly inside `linear-gradient()`, it is suggested to either calculate a fixed pixel value beforehand or use alternative positioning methods.