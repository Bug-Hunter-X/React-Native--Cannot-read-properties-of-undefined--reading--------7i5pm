# React Native: Handling 'Cannot read properties of undefined' Errors

This repository demonstrates a common error in React Native: the dreaded 'Cannot read properties of undefined (reading '...')' error.  This occurs when attempting to access a property of an object that is currently null or undefined.  The example showcases the problem and its solution using optional chaining and nullish coalescing.

## Problem

The `bug.js` file contains a React component that fetches user data asynchronously.  Before the data is fetched, the `user` object is null.  Attempting to access `user.name` directly results in the 'Cannot read properties of undefined' error.

## Solution

The `bugSolution.js` file demonstrates how to gracefully handle this situation using optional chaining (`?.`) and the nullish coalescing operator (`??`).  These features prevent the error by short-circuiting the property access if the object or a nested property is null or undefined.