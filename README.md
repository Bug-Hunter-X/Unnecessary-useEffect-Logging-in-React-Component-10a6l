# Unnecessary useEffect Logging in React Component

This repository demonstrates a common React bug involving the `useEffect` hook. The component's `useEffect` hook logs a message on every render, even though the dependency array seems correctly configured.

The bug stems from a misunderstanding of how `useEffect` with an empty dependency array works, and how state updates might trigger unexpected re-renders.

## Bug

The provided `bug.js` contains a React component that demonstrates the issue. The `useEffect` hook logs the current count every time the component re-renders, regardless of whether the count actually changes. This is inefficient and may lead to performance issues.

## Solution

The `bugSolution.js` file provides a fix for this problem. By removing the unnecessary logging and optimizing the `useEffect` use, the bug is resolved, leading to increased performance and cleaner code.

## How to reproduce

Clone this repository and run:

```
npm install
npm start
```
This will start the React development server and let you interact with the component and observe the behavior.

## Further considerations

This example highlights the importance of understanding how the dependency array in `useEffect` works. Proper use of dependencies is essential for writing performant and predictable React applications.