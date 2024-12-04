# Missing Catch-All Route in React Router v6

This repository demonstrates a common error in React Router v6: forgetting to include a catch-all route (`/*`) to handle unexpected or invalid paths.  Without this route, the application may not handle navigation to non-existent pages gracefully.

## The Bug
The `App.js` file shows an incomplete route configuration.  It defines routes for `/` and `/about`, but lacks a route to handle any other path.  This means that navigating to a non-existent route will result in the application showing nothing (blank screen) instead of a proper 'Not Found' page.

## The Solution
The `AppSolution.js` file demonstrates the corrected version with a catch-all route (`/*`) added.  This route ensures that a designated component (in this case, `NotFound`) is displayed for any invalid or unknown paths.