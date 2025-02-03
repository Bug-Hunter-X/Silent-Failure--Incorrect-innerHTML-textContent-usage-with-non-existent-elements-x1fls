# Uncommon HTML Bug: Silent Failure with Non-Existent Elements

This repository demonstrates a subtle bug in HTML that can lead to unexpected behavior. The code attempts to modify the `innerHTML` and `textContent` of elements that do not exist in the Document Object Model (DOM).  This results in a silent failure; no error is thrown, but the intended changes do not occur.

The bug highlights the importance of verifying the existence of elements before manipulating them using methods like `innerHTML` and `textContent`.

## Bug Details
The `bug.html` file contains the erroneous code.  It tries to set the `innerHTML` of a non-existent element, and then `textContent`, again on a non existent element which will cause a runtime error.  This demonstrates a case where a runtime error may not be caught by simple testing.