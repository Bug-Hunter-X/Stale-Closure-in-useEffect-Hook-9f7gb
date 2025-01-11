# Stale Closure in React's useEffect Hook

This repository demonstrates a common error in React applications involving stale closures within the `useEffect` hook.  When using state variables within a function declared inside `useEffect`, it's crucial to understand that the function doesn't capture the *live* state value, but rather a snapshot of its value at the time the effect was created.

The `bug.js` file shows the incorrect implementation, resulting in an inaccurate counter. The `bugSolution.js` file presents the corrected code, resolving the stale closure issue.

## How to Reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Open `bug.js` to see the faulty implementation.
4. Open `bugSolution.js` to see the corrected implementation. 

This example highlights the importance of ensuring that state updates are correctly handled within effects to avoid unexpected behavior.