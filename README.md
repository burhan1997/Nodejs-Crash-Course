# NODEJS Crash Course

Welcome to the Node.js Crash Course! In this crash course, we will delve into Node.js fundamentals, covering modules such as `path`, `url`, `fs`, and `events`. Additionally, we will walk through the process of creating an HTTP server from scratch without relying on Express.

## What is Node.JS?

- Javascript Runtime (NOT a language or framework)
- Built on the V8 Javascript engine (Same as Google Chrome)
- Written in C++
- Essentially allows us to run Javascript code on the server

## Why Use Node?

- Fast, efficient, and highly scalable
- Event-driven, non-blocking I/O model
- Popular in the industry
- Consistent language on the front and back end (JS)

## Non-Blocking I/O

- Works on a single thread using non-blocking I/O calls
- Supports tens of thousands of concurrent connections
- Optimizes throughput & scalability in apps with many I/O operations
- All of this makes Node.js apps very fast & efficient

## Node's Event Loop

- Single-threaded
- Supports concurrency via events & callbacks
- `EventEmitter` class is used to bind events and listeners
- When Node.js starts, it initializes the event loop, processes the provided input script which may make async API calls, schedule timers, or call `process.nextTick()`, then begins processing the event loop.

## Best Types of Projects for Node

- REST API & Microservices
- Real-Time Services (Chat, Live Updates)
- Blogs, Shopping Carts, Social Networks
- Short answer: Anything that is not CPU intensive

## NPM - Node Package Manager

- Install 3rd party libraries (frameworks, libraries, tools, etc)
- Packages get stored in the "node_modules" folder
- All dependencies are listed in a "package.json" file
- NPM scripts can be created to run certain tasks such as running a server

```javasccript
npm init --> Generates a package.json file
npm install express --> Installs a package locally
npm install -g nodemon --> Installs a package globally
```

## Node Modules 
- Node Core Modules (paths, fs, http, etc.)
- 3rd party modules/packages installed via NPM
- Custom modules (files)

```javascript
const path = require('path');
const myFile = require('./myFile')
