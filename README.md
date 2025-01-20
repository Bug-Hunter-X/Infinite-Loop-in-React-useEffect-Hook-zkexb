# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug is caused by omitting dependencies in the `useEffect` hook's dependency array, leading to an infinite render loop. The solution showcases the correct way to add dependencies to prevent this issue.

## Bug Description

The `useEffect` hook is intended to perform side effects after a render. If the dependency array is missing or empty, the effect runs after every render, creating an infinite loop. This example showcases such a scenario.

## Solution

The solution correctly specifies the `count` state variable in the dependency array, ensuring that the effect runs only when `count` changes.