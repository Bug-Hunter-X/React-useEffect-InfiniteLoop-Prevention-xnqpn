# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug occurs when a dependency is missing from the useEffect hook's dependency array. This leads to an infinite render loop because the effect runs after every render and causes a state update that triggers another render. 

## Bug
The `bug.js` file contains the buggy code. It showcases the incorrect implementation of the `useEffect` hook, where the `count` variable isn't listed as a dependency in the dependency array, therefore leading to an infinite loop.