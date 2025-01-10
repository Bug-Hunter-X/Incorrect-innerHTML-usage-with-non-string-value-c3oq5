# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates an uncommon bug in HTML related to the `innerHTML` property.  The bug arises from attempting to set the `innerHTML` property of an element to a non-string value (in this case, a number). This can lead to unexpected behavior in the browser.

## Bug Description:
The provided HTML code uses `document.getElementById("myDiv").innerHTML = 123;`  This sets the `innerHTML` to the number 123 instead of the expected string representation of 123. 

## Solution:
The solution involves ensuring that you always assign a string value to the `innerHTML` property. This can be done by explicitly converting the number to a string using String() or by using template literals.

## How to Reproduce:
1. Clone this repository.
2. Open `bug.html` in your web browser.  Observe that the content of the div may not be correctly updated.
3. Open `bugSolution.html` to see the corrected version.