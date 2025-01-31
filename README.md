# React Native useEffect Infinite Loop with Function Dependency

This repository demonstrates a common error in React Native: an infinite loop caused by using a function as a dependency in the `useEffect` hook. The bug involves asynchronous operations within the `useEffect`, making the issue more difficult to diagnose.

The `useEffectBug.js` file shows the buggy code. The `useEffectSolution.js` file provides the corrected code using `useCallback` to memoize the function and prevent the infinite loop.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npx react-native run-android` (or `npx react-native run-ios`).
4. Observe the infinite loop and subsequent errors in the buggy example.
5. Compare the solution to see how `useCallback` fixes the problem.