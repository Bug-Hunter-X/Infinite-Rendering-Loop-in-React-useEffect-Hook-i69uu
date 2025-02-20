# React Infinite Rendering Bug

This repository demonstrates a common React bug involving infinite rendering loops caused by the misuse of the `useEffect` hook.

## Bug Description
The `MyComponent` uses `useEffect` to log the current count to the console after each render.  However, it omits the dependency array, causing the effect to re-run after every state update, leading to an infinite loop of renders and console logs.