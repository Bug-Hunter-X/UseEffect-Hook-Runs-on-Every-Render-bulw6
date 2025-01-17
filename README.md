# React useEffect Hook Runs on Every Render

This repository demonstrates a common issue with the React `useEffect` hook where it runs on every render instead of only when its dependencies change.  This can lead to performance problems, especially in complex components.

## Problem
The provided `MyComponent` uses `useEffect` without specifying dependencies correctly. This causes the effect to run after every render, leading to unnecessary logging and potential performance issues.

## Solution
The solution involves correctly specifying the dependencies array in `useEffect`.  By passing `[count]` as the dependency array, the effect only runs when the value of the `count` state variable changes.