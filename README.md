# Uncommon HTML Bug: innerHTML on Non-Existent Element

This repository demonstrates a subtle HTML bug that can occur when using `innerHTML` to modify a DOM element that does not yet exist. The bug is that the javascript execution will continue even if there is an error in accessing the dom element. 

The `bug.html` file contains the buggy code. The `bugSolution.html` file provides a corrected version.

## Bug

The original code attempts to set the `innerHTML` property of a non-existent element. This will not throw an error but result in no change. The solution shows the correct way of handling this situation.

## Solution

The solution uses error handling to gracefully address the case of a missing element. 
