Question 1 : What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

Ans:

* getElementById: Selects a single element using its unique id. Returns that element or null if it does not exist.

* getElementsByClassName: Selects all elements with a given class name. Returns a live HTMLCollection, which updates when the DOM changes.

* querySelector: Finds the first element that matches a CSS selector. Returns the element or null if none is found.

* querySelectorAll: Finds all elements that match a CSS selector and returns a static NodeList, which does not change automatically if the DOM updates.

Question 2 : How do you create and insert a new element into the DOM?

Ans:
 We create a new DOM element using document.createElement("tagName"). After that, we can insert it into the page using methods such as:

* appendChild() → Adds the element as the last child of a parent.

* prepend() → Inserts it as the first child.

* insertBefore() → Places it before a specific existing node.

Question 3 : What is Event Bubbling and how does it work?

Ans:
Event bubbling is the process where an event triggered on a child element first executes its own handler, and then propagates upward to its parent, grandparent, the document, and finally the window.

Question 4 : What is Event Delegation in JavaScript? Why is it useful?

Ans:
Event Delegation is a pattern where instead of attaching listeners to many child elements, we attach a single listener to a parent element. Since events bubble up, the parent can detect which child triggered the event.

Benefits:

* Improves performance by reducing the number of listeners.

* Works well for dynamically created elements.

* Makes the code cleaner and easier to maintain.

Question 5 : What is the difference between preventDefault() and stopPropagation() methods?

Ans:

* preventDefault(): Cancels the browser’s default behavior for the event (e.g., stopping a link from navigating, preventing form submission).

* stopPropagation(): Prevents the event from bubbling up the DOM, so parent element listeners won’t be triggered.