# JavaScript TypeError: Cannot read properties of undefined (reading 'length')

This repository demonstrates a common JavaScript error: `TypeError: Cannot read properties of undefined (reading 'length')`.  The error arises when code attempts to access the `length` property of a variable that is currently undefined.

The `bug.js` file contains the problematic code.  The `bugSolution.js` file provides a corrected version.

## How to reproduce

1. Clone the repository.
2. Navigate to the directory.
3. Run `node bug.js` in your terminal.  Observe the error.
4. Run `node bugSolution.js` to see the corrected behavior.

## Problem Description

The original code attempts to handle `null` values gracefully, but fails to account for `undefined`.  Accessing the `length` property of `undefined` results in the `TypeError`.

## Solution

The solution explicitly checks for both `null` and `undefined` before accessing the `length` property, preventing the error.