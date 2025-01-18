# Uncommon DOM Manipulation Bug: Accessing Removed Element

This repository demonstrates an uncommon bug related to DOM manipulation in HTML and JavaScript.  The bug arises when you attempt to access and modify a DOM element that has already been removed from the DOM tree using the `remove()` method.

## Bug Description

The `bug.html` file contains a simple HTML structure with a div and a button. The JavaScript function removes the div from the DOM and then attempts to re-add content to it. This causes an error because the element reference is no longer valid.

## Solution

The `bugSolution.html` file provides a solution by checking if the element exists in the DOM before attempting to modify it.  Alternatively, re-creating the element is safer.

## How to reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Click the button.  Observe the error in your browser's developer console.
4. Open `bugSolution.html` and observe the correct behaviour.