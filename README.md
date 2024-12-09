# JavaScript Loose Equality Bug
This repository demonstrates a common, yet subtle, bug in JavaScript related to the misuse of loose equality (`==`) when checking for null values.  The bug arises when loose equality is used, leading to unexpected behavior with other falsy values.  Strict equality (`===`) provides a more precise comparison.

## Bug Description
The provided JavaScript code snippet checks for null values using loose equality (`==`). This causes unexpected behavior when values that are falsy but not null (e.g., 0, "") are passed as arguments. Strict equality (`===`) avoids this issue.

## Solution
The solution replaces loose equality (`==`) with strict equality (`===`) to ensure that only null values are handled correctly.

## How to reproduce
1. Clone this repository.
2. Navigate to the root directory.
3. Run the `bug.js` file using a JavaScript interpreter (e.g., Node.js). Observe the unexpected behavior when passing falsy values other than null.
4. Run the `bugSolution.js` file to see the corrected version.

