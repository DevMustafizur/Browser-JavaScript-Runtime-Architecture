# Browser Javascript Runtime

### 1. What is Browser JavaScript Runtime?

Answer: Browser JavaScript Runtime is the complete environment where JavaScript executes and can use browser features.

### 2. What are the main components of Browser Runtime?

Answer:

- JavaScript Engine
- Window Object
- Browser/Web APIs
- Task Queue
- Microtask Queue
- Event Loop
- Browser Native Implementation
  
### 3. What is a JavaScript Engine?

Answer: A JavaScript Engine parses, compiles, and executes JavaScript code. Example: V8.

### 4. What is the Window Object?

Answer: The window object is the browser's global object. It provides access to objects such as document, location, and navigator.

### 5. What are Browser/Web APIs?

Answer: Browser APIs are browser-provided features such as DOM, Fetch, Timers, Storage, and Events.

### 6. What is the Task Queue?

Answer: The Task Queue holds tasks and callbacks waiting for execution, such as setTimeout() and UI event callbacks.

### 7. What is the Microtask Queue?

Answer: The Microtask Queue holds microtasks such as Promise callbacks and queueMicrotask().

### 8. What is the Event Loop?

Answer: The Event Loop coordinates JavaScript execution with the Task Queue and Microtask Queue.

### 9. Where does JavaScript execute in the Browser?

Answer: JavaScript executes inside the JavaScript Engine, such as V8 in Chrome.

### 10. What is the difference between Engine and Runtime?

Answer:

Engine  = Executes JavaScript
Runtime = Engine + APIs + Queues + Event Loop
### 11. What is the relationship between ECMAScript and Browser Runtime?

Answer: ECMAScript defines the JavaScript language, while the Browser Runtime provides the environment and browser APIs to run it.

### 12. How does setTimeout() work?

Answer: The browser handles the timer → the callback enters the Task Queue → the Event Loop allows it to execute in the JavaScript Engine.

### 13. How do Promises work?

Answer: Promise callbacks are placed in the Microtask Queue and processed after the current JavaScript execution completes.

### 14. Does Browser Runtime consist only of V8?

Answer: No. V8 is only the JavaScript Engine. The Browser Runtime also includes APIs, queues, the Event Loop, and native browser implementation.

### 15. What does the Browser provide to JavaScript?

Answer: The browser provides features such as DOM, Fetch, Timers, Storage, Events, and Geolocation.

