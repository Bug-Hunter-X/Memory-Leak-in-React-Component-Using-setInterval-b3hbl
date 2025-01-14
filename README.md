# React setInterval Memory Leak

This repository demonstrates a common React bug: a memory leak caused by the improper use of `setInterval` within a `useEffect` hook.  The provided `bug.js` file shows the problematic code.  The solution, shown in `bugSolution.js`, addresses the leak by correctly clearing the interval using the cleanup function returned by `useEffect`.

## How to Reproduce

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install`.
4. Run `npm start`.
5. Observe the continuously increasing counter, which indicates a memory leak in the `bug.js` example.
6. Switch to the `bugSolution.js` example which properly cleans up the interval.