# React useEffect Hook Missing Dependency
This repository demonstrates a common error in React applications: a missing dependency in the useEffect hook.  The effect runs after every render instead of only when the value it depends on changes.

## Problem
The initial code example shows an incorrect use of useEffect.  Without the `count` variable in the dependency array, the effect runs on every render, resulting in excessive logging and potentially unexpected side effects.

## Solution
The solution demonstrates the correct usage of useEffect, including the `count` variable in the dependency array.  This ensures the effect runs only when the `count` value changes.

## How to reproduce
1. Clone the repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs to see the effect's behavior in the incorrect and corrected versions.