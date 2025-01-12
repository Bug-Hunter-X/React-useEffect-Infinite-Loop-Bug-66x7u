# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: creating an infinite loop by incorrectly specifying dependencies.

The `bug.js` file contains code that leads to this error. The `bugSolution.js` file shows the correct implementation.

## How to reproduce the bug

1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the infinite loop in the console and the rapidly changing counter.

## Solution

The solution involves understanding how the dependency array in useEffect works.  The corrected code in `bugSolution.js` removes the unnecessary dependency on the `count` variable.