# Express.js Route Handler Error
This repository demonstrates a common error in Express.js route handlers:  missing error handling for invalid input and missing 404 responses for non-existent resources.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version.

## Bug Description
The original code lacks error handling for scenarios where:

1.  The user ID (`req.params.id`) is not a valid number.
2.  A user with the specified ID does not exist.

These omissions can lead to unexpected behavior or crashes.

## Solution
The solution includes robust error handling. It checks if the user ID is a number and handles the scenario where a user is not found using an appropriate 404 response.