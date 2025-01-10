# Unhandled 'error' event in Node.js HTTP server

This repository demonstrates a common Node.js error: an unhandled 'error' event. The error occurs when an unexpected problem arises within an asynchronous operation, such as a network request or file system operation.  If not handled, it will cause the Node.js process to crash.

## Bug
The `bug.js` file contains a simple HTTP server that lacks error handling.  When the server encounters an error (e.g., a connection problem), the process will unexpectedly terminate without logging any useful information.

## Solution
The `bugSolution.js` file demonstrates how to properly handle this error by using the `'error'` event listener. This ensures that the server gracefully handles errors and prevents unexpected crashes.