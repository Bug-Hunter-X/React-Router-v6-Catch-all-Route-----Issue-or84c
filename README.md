# React Router v6 Catch-all Route (*) Issue

This repository demonstrates a common issue encountered when using the catch-all route (`*`) in React Router v6.  The issue is that the catch-all route sometimes prevents other routes from working correctly, leading to unexpected behavior.  The solution involves carefully considering the order of routes and potentially using a more specific catch-all route.

## Problem

The provided `App.js` contains a basic React Router setup with a home route, an about route, and a catch-all route for handling 404 errors. However, the catch-all route is incorrectly overriding the other routes, causing them to be inaccessible.

## Solution

The `AppSolution.js` file provides a corrected version of the code. The solution ensures that the catch-all route is placed last in the `Routes` component, ensuring that it only matches if no other route matches.  This is the correct behavior for catch-all routes within `Routes`.
