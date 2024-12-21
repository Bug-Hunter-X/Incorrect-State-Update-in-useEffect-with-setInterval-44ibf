# Incorrect State Update in useEffect with setInterval

This repository demonstrates a common mistake when using the `useEffect` hook with `setInterval` in React.  The issue arises from incorrectly managing state updates within the closure created by the `useEffect` hook.  The provided code initially demonstrates the bug, while the solution showcases the correct approach to update state based on the previous value.

## Bug

The `bug.js` file shows how using `setCount(count + 1)` within `setInterval` leads to stale closures, resulting in inaccurate state updates that are not reflecting the most recent state.