# Missing Revert Condition for Hidden Element

This repository demonstrates a common yet easily overlooked bug in HTML/JavaScript.  A div element is hidden when a button is clicked, however there is no mechanism provided to make the div visible again. This leads to a permanent disappearance of the element.

## Bug Description
The issue lies within the `myFunction()` JavaScript function. It hides the div element with `style.display = "none";` but it does not provide a way to make it visible again.  This is a subtle error that can be hard to debug if not carefully examined.

## Solution
The solution involves adding a simple conditional to the javascript function to re-display the element.