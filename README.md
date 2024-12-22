# React Router v6 Missing Route Handling

This repository demonstrates a common issue in React Router v6: the lack of a default route or a 404 page when navigating to a non-existent path.  The application will appear to break when you try to access a URL that doesn't have a corresponding Route component defined.

## Problem:

The provided `App.js` shows a basic React Router setup. Notice that there's no route defined for `/contact`.  Navigating to `/contact` will result in a blank screen or unexpected behavior because React Router doesn't know how to handle this path.

## Solution:

The `AppSolution.js` demonstrates two common solutions:

1. **Adding a catch-all route:** Adding a route with `path="*"` acts as a 404 page, displaying content when no other routes match.
2. **Using `useLocation` hook for custom error handling:** You can use the hook to detect errors and render your own custom error page.

This repository offers clear examples of how to solve this problem and improve your app's user experience.