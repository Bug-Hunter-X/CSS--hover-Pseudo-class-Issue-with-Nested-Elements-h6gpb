# CSS :hover Pseudo-class Issue with Nested Elements

This repository demonstrates a subtle bug related to the `:hover` pseudo-class in CSS when applied to nested elements. The issue arises from the specificity of CSS selectors and how styles cascade.  The provided example shows a scenario where the inner element's style fails to change on hover of the outer element, despite seemingly correct CSS.

The `bug.css` file contains the buggy CSS code.  The `bugSolution.css` demonstrates how to resolve this issue.

## Reproducing the Bug

1. Open `bug.html` (or create your own HTML to include the provided CSS).
2. Observe that the inner green square does not change color when you hover over the outer blue square.

## Solution

The solution involves ensuring the specificity of the `:hover` selector is high enough to override the existing style on the inner element.  This is achieved in the `bugSolution.css` file.