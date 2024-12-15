# Uncommon HTML Error: Unexpected innerHTML behavior
This repository demonstrates an uncommon error related to the `innerHTML` property in HTML.  The error arises from attempting to set the `innerHTML` property of an element to a non-string value. While many developers are familiar with common HTML errors like syntax issues or missing closing tags, this example highlights a less frequently encountered problem involving type coercion within JavaScript and its effects on the DOM manipulation.

The `bug.html` file contains the erroneous code. The `bugSolution.html` file provides the corrected version.

## How to reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the unexpected behavior or error in the browser's console.
4. Open `bugSolution.html` to see the corrected code and the expected output.

## How to solve
Always ensure that the value assigned to `innerHTML` is a string. Type coercion might lead to unexpected results, making explicit string conversion necessary for reliable behavior. The solution involves converting the number to a string using the `toString()` method before assigning it to `innerHTML`.