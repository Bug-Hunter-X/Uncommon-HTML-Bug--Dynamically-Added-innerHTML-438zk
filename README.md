# Uncommon HTML Bug: Dynamically Added innerHTML

This repository demonstrates an uncommon bug related to dynamically adding innerHTML to an element in HTML.  The bug, present in `bug.html`, highlights the issue of trying to manipulate elements before they're fully rendered. The solution is presented in `bugSolution.html`.

## Bug Description
The primary issue lies in the JavaScript code which attempts to add innerHTML to an element that might not be fully parsed or attached to the DOM. This can lead to unexpected results or errors.

## Solution
The solution demonstrates a common practice of ensuring the element exists in the DOM tree by using `addEventListener('DOMContentLoaded', ...)` before attempting the innerHTML manipulation. This guarantees the element is ready and available for modification.

## How to reproduce the bug
1. Open `bug.html` in your web browser.
2. Observe the unexpected behavior, potentially an empty `div` element or a JavaScript error.

## How to observe the solution
1. Open `bugSolution.html` in your web browser.
2. Notice that the innerHTML is successfully added to the `div` element without error.