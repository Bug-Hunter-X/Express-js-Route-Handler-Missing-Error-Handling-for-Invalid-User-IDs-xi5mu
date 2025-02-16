# Express.js Route Handler Missing Error Handling for Invalid User IDs

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input parameters.  The example focuses on handling user IDs, but the concept applies to any input that needs validation.

## Bug Description

The provided `bug.js` file contains an Express.js route handler that retrieves a user by their ID. It attempts to parse the ID as an integer using `parseInt()`, but it doesn't handle cases where the ID is not a valid integer (e.g., it's a string or contains non-numeric characters).  This can lead to errors, unexpected behavior, or even application crashes.

## Solution

The `bugSolution.js` file provides a solution by adding robust error handling.  It checks if the ID is a valid integer and responds appropriately if it's not.  This prevents unexpected errors and improves the application's stability and reliability.