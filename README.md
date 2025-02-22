# Node.js Server Hang During Long Operation

This repository demonstrates a common issue in Node.js where long-running operations can block the event loop, causing the server to become unresponsive. The `bug.js` file contains a server that simulates a long-running task using a busy-wait loop. This blocks the event loop, preventing it from handling other requests and causing the server to hang.

The `bugSolution.js` file demonstrates a solution using asynchronous operations with `setTimeout` to avoid blocking the event loop and keep the server responsive.