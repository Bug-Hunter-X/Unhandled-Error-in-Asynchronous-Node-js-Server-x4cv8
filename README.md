# Unhandled Error in Asynchronous Node.js Server

This repository demonstrates a common error in Node.js server development: unhandled errors within asynchronous operations inside request handlers.

## The Problem

Asynchronous operations, such as those using `setTimeout` or database queries, can throw errors that are not immediately caught within the request handler. If not handled properly, these errors can cause the server to crash, leading to downtime and instability.

## The Solution

The solution involves carefully handling potential errors within asynchronous callbacks or using `async/await` with `try...catch` blocks.  The provided example shows how to implement proper error handling using server's 'error' event.

## How to Run

1. Clone the repository.
2. Navigate to the repository's directory.
3. Run `node bug.js` to see the unhandled error.
4. Run `node bugSolution.js` to see the implemented solution with proper error handling.