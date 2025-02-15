# CSS Specificity Bug: Hover Issue

This repository demonstrates a common CSS specificity issue that can lead to unexpected behavior with the `:hover` pseudo-class.  The problem arises when a more specific selector unintentionally overrides the hover style.

## Bug Description:

A hover effect on a link is not applied as expected.  This is caused by a specificity conflict between the base link style and styles applied to the link within a container, resulting in the container's styles overriding the hover effect.

## Solution:

The solution involves increasing the specificity of the hover selector to ensure it takes precedence.  See `bugSolution.css` for the corrected code.

## How to reproduce:

1. Clone this repository
2. Open `bug.html` in your browser.
3. Hover over the link. You'll see the default color, rather than the hover color.
4. Open `bugSolution.html` and hover over the link. You will see the hover effect work correctly. 