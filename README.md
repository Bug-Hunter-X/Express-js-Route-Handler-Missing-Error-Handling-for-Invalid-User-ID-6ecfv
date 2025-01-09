# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  missing error handling for invalid input.  Specifically, the `/users/:id` route attempts to parse the `id` parameter as an integer without checking if it's actually a valid number. This can cause unexpected behavior or crashes if the `id` is not a number.

## Bug

The `bug.js` file contains the flawed code. It attempts to find a user by ID but doesn't handle cases where the ID is not a valid integer.

## Solution

The `bugSolution.js` file provides a corrected version of the code. It includes error handling to check if the ID is a valid integer and handles the case where the user is not found.