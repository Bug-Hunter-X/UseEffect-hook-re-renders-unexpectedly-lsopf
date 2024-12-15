# React useEffect Hook Unexpected Re-renders

This repository demonstrates a common issue with the React `useEffect` hook where it re-renders more frequently than expected, even with a seemingly correct dependency array.

## Bug Description

The `useEffect` hook in the provided `MyComponent` function is intended to log the current count to the console only when the `count` state variable changes.  However, it's logging on every render, leading to performance issues and potentially unexpected behavior. 

## Solution

The solution involves correctly using the dependency array to ensure the effect only runs when the dependencies change.