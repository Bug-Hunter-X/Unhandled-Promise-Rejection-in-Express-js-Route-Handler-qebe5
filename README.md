# Unhandled Promise Rejection in Express.js Route Handler

This repository demonstrates a common error in Express.js applications: unhandled promise rejections.  The `bug.js` file contains code with an asynchronous operation in a route handler that lacks proper error handling.  This can lead to unexpected application crashes and instability.

The `bugSolution.js` file provides a corrected version with robust error handling to prevent these issues.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `npm install express` to install the required dependency.
4. Run `node bug.js`. Observe that there is no output and the server may crash (due to the unhandled promise rejection).
5. Run `node bugSolution.js`. The server will start without any unhandled rejection.