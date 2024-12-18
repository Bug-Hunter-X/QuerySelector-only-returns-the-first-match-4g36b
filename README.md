# Uncommon HTML Bug: querySelector and Multiple Elements

This repository demonstrates a subtle bug related to using `document.querySelector` in HTML/JavaScript. The script intends to style multiple paragraphs, but only modifies the first one found.

## Bug Description

The `querySelector` method only selects the first element that matches the provided selector.  If you intend to style multiple elements, you'll need to use `querySelectorAll`. This difference can easily be overlooked, leading to unexpected behavior.

## Solution

The solution involves replacing `querySelector` with `querySelectorAll` and iterating through the results to apply the styling to each element individually.