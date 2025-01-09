# Uninitialized State/Prop Access in React Native

This repository demonstrates a common error in React Native: attempting to access state variables or props before they have been properly initialized. This often leads to unexpected behavior or crashes, especially when dealing with asynchronous operations.

## The Problem
The `bug.js` file showcases the issue: accessing the `data.name` property before the asynchronous `fetch` call completes and sets the `data` state variable.  This will cause a runtime error because `data` is initially `null`.

## The Solution
The `bugSolution.js` demonstrates how to correctly handle this by using optional chaining and a null check to prevent errors.   This is a best practice to always handle potentially null or undefined values when accessing them from state or props. 

## How to Run
1. Clone the repository
2. Navigate to the directory in your terminal.
3. Run `npm install` to install the dependencies.
4. Run `npx react-native run-android` (or `npx react-native run-ios`) to run the app.