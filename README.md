# Unhandled Exception in Node.js HTTP Server

This repository demonstrates a common error in Node.js applications: unhandled exceptions in HTTP servers.  Improper error handling can lead to unexpected crashes and disruptions in service.

The `bug.js` file shows a server that throws an unhandled exception when accessing the `/error` route.  The `bugSolution.js` file demonstrates the proper way to handle errors and gracefully respond.

## How to reproduce the bug:

1. Clone this repository.
2. Run `node bug.js`.
3. Access `http://localhost:3000/error` in your browser or using a tool like `curl`.
4. Observe the server crashing.

## How to fix the bug:

Refer to `bugSolution.js` for a corrected version that includes proper error handling. The key change involves using a `try...catch` block to handle potential exceptions and prevent the server from crashing.