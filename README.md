# React 19 useEffect Infinite Loop Bug

This repository demonstrates a common error in React 19 related to the useEffect hook.  Incorrectly specifying dependencies in useEffect can lead to an infinite loop, causing performance issues and potentially crashing the application. The bug and its solution are illustrated using simple code examples.

## Bug Description:
The `useEffect` hook, when used without a dependency array or with an incorrect dependency array, will run after every render. This can trigger unintended side effects (like infinite loops) if not managed properly. This is especially relevant in React 19 with its improved performance optimizations.

## How to Reproduce:
1. Clone the repository
2. Run `npm install`
3. Run `npm start`
4. Observe the console output and the continuous re-rendering in your browser's developer tools.

## Solution:
The solution involves correctly specifying the dependency array in `useEffect` to only run the effect when specific values change. 