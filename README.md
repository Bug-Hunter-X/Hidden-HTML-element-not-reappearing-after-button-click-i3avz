# Hidden HTML Element Bug

This repository demonstrates a simple HTML bug where a div element is hidden using JavaScript after a button click, but never reappears.  The solution demonstrates how to correctly restore the visibility of the element.

The bug is caused by not adding code to re-enable the display of the hidden element after the initial hide operation. This can lead to UI elements becoming permanently invisible and confusing the user experience.

## Bug Description

When the user clicks the button, the `myDiv` element is hidden using JavaScript's `style.display = "none";`.  However, there's no subsequent code to set `style.display` back to its default, resulting in the div remaining hidden indefinitely.

## Solution

The solution involves adding a `setTimeout` function to restore the display property after a delay, allowing the element to reappear.