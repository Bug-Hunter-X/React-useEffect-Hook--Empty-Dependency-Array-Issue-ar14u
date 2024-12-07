# React useEffect Hook: Empty Dependency Array Issue

This example demonstrates a common mistake when using the `useEffect` hook in React. The empty dependency array `[]` causes the effect to only run once when the component mounts and again when it unmounts.  This prevents the effect from responding to changes in state.

## Problem:
The `useEffect` with `[]` does not update when `count` changes. The console log only shows the initial count. 

## Solution:
Include `count` in the dependency array to trigger the effect whenever `count` updates. 