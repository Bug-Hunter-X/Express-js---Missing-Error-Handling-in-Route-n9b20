# Express.js - Missing Error Handling in Route

This example demonstrates a common error in Express.js applications: missing error handling for invalid user IDs.  The code attempts to find a user by ID, but doesn't handle the case where the user is not found, leading to potential crashes or unexpected behavior.

## Bug
The `bug.js` file showcases the problematic code.  When a user with a non-existent ID is requested, the application doesn't return a proper error response (e.g., a 404 Not Found), but instead throws an error if it cannot find the user.

## Solution
The `bugSolution.js` file provides a corrected version. It explicitly checks if the user exists, sending a 404 response if not found. This ensures a more robust and user-friendly experience.
