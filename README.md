# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js where a long-running synchronous operation in the request handler blocks the event loop, causing the server to become unresponsive.  The solution showcases how to address this using asynchronous operations.

## Bug
The `server.js` file contains a simple HTTP server that simulates a long-running task within the request handler. This blocks the event loop, preventing the server from handling subsequent requests.

## Solution
The `serverSolution.js` file provides a solution that uses asynchronous operations to prevent blocking the event loop.  This ensures the server remains responsive even under heavy load.

## How to run

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `node server.js` to observe the unresponsive behavior.
4. Run `node serverSolution.js` to see the improved responsiveness.