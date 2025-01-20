# React useEffect Infinite Loop

This repository demonstrates a common React bug: an infinite loop caused by improperly using the `useEffect` hook.  The `useEffect` hook's callback updates the state, which triggers a re-render, leading to a continuous cycle of updates.

## Bug
The `bug.js` file contains a component that attempts to increment a counter within the `useEffect` hook, without the proper dependency array conditions to prevent an infinite loop. 

## Solution
The `bugSolution.js` file provides the correct implementation of useEffect for handling this scenario, illustrating the correct way to manage state changes within the useEffect hook to prevent infinite loops.

## How to Reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`. 
4. Observe the behavior in the console and how it differs between the buggy and fixed versions.