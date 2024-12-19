# CSS Float and Auto Width Issue

This repository demonstrates an uncommon issue related to using floats and auto width in CSS.  Some browsers behave unexpectedly when a floated element's width is set as a percentage of an automatically sized parent container.

The problem arises because the auto width of the parent is resolved *before* the percentage width of the children is calculated, causing the result to be unexpectedly small. This is not consistent across all browsers, leading to inconsistencies in layout.

The `bug.css` file contains the problematic CSS, and `bugSolution.css` demonstrates a solution to resolve the issue.