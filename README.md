This repository demonstrates an uncommon bug in HTML where an element's display property is set to 'none' using JavaScript before the element is fully rendered by the browser. This results in the element being completely invisible, even though it exists in the DOM.

The bug is demonstrated in the `bug.html` file. The solution is to either move the JavaScript code that sets the `display` property to after the element in the HTML, or to use `setTimeout` to delay the execution of this code. The solution is demonstrated in `bugSolution.html`.

This bug is subtle and can be difficult to diagnose, as the element technically exists in the DOM but is never shown to the user.