# 1. What is Browser JavaScript Runtime?

The Browser JavaScript Runtime is the complete environment provided by a browser where JavaScript code executes and can use browser features such as DOM, Timers, Network, Storage, and Events.

Browser JavaScript Runtime
│
├── V8 JavaScript Engine
├── Browser APIs
├── Window Object
├── Task Queues
└── Event Loop

Runtime = V8 Engine + Browser APIs + Window Object + Queues + Event Loop

---

# 2. JavaScript Runtime vs JavaScript Engine

JavaScript Engine: Executes JavaScript code. Example: V8.

JavaScript Runtime: A complete environment for running JavaScript, including the engine, APIs, queues, and event loop.

Engine  = Executes JavaScript
Runtime = Engine + APIs + Queues + Event Loop


---



### 3 What is the relationship between ECMAScript and the Browser Runtime?

**ECMAScript** defines the JavaScript language and its built-in features, while the **Browser Runtime** provides the environment and Web APIs to run JavaScript.

```text
ECMAScript → JavaScript Language Specification
Browser Runtime → v8 + Browser APIs + window + Event Loop + Queues
```

---


### 4. What are the main components of a Browser Runtime?

The main components are:

* **V8 JavaScript Engine**
* **Browser APIs**
* **Window Object**
* **Task Queues**
* **Event Loop**

---

## 5. What is the role of the JavaScript Engine in the Browser Runtime?

**Answer:** The JavaScript Engine parses, compiles, and executes JavaScript code. In Chrome, the engine is **V8**.

---

## 6. What are Browser APIs?

**Answer:** Browser APIs are features provided by the browser that JavaScript can use, such as DOM, Fetch, Timers, Storage, and Events.

---

## 7. What is the Window Object?

**Answer:** The `Window` object represents the browser window and acts as the global object in browser JavaScript.

---

## 8. What is the role of the Window Object in the Browser Runtime?

**Answer:** The `Window` object provides access to browser-related objects and APIs such as `document`, `location`, `history`, `navigator`, and timers.

---

## 9. What are Task Queues?

**Answer:** Task Queues store callbacks that are waiting to be executed by the JavaScript runtime.

---

## 10. What is the Event Loop?

**Answer:** The Event Loop checks whether the JavaScript execution stack is empty and moves waiting callbacks from queues to the stack for execution.

---

## 11. How does the Event Loop work?

**Answer:** The Event Loop checks the call stack and queues. When the stack is empty, it moves eligible queued callbacks to the stack for execution.

---

## 12. Where does JavaScript code execute in the Browser?

**Answer:** JavaScript code executes inside the **JavaScript Engine**, such as V8. The Browser Runtime provides the surrounding APIs and event-handling environment.

---

## 13. Does the Browser Runtime consist only of V8?

**Answer:** No. V8 is only the JavaScript Engine. The Browser Runtime also includes Browser APIs, Window Object, Queues, and the Event Loop.

---

## 14. What does the Browser provide to JavaScript?

**Answer:** The browser provides Web APIs such as DOM, Fetch, Timers, Storage, Events, and other browser-specific features.

---

## 15. What is the difference between Browser APIs and ECMAScript?

**Answer:** ECMAScript defines the JavaScript language and built-in features, while Browser APIs provide browser-specific features such as DOM, Fetch, and Timers.

---

## 16. How do Browser APIs and JavaScript Engine work together?

**Answer:** JavaScript executes in the engine, while Browser APIs handle browser-specific operations and provide results or callbacks to the runtime.

---

## 17. What is the role of Queues in the Browser Runtime?

**Answer:** Queues hold callbacks and jobs that are waiting for execution by the JavaScript Engine.

---

## 18. What is the difference between Task Queue and Microtask Queue?

**Answer:** The Task Queue handles tasks such as timer and event callbacks, while the Microtask Queue handles jobs such as Promise callbacks.

---

## 19. How do Promises work in the Browser Runtime?

**Answer:** Promise callbacks are placed in the **Microtask Queue** and are processed after the current JavaScript execution completes.

---

## 20. How does `setTimeout()` work in the Browser Runtime?

**Answer:** The browser handles the timer. When the timer is ready, its callback is placed in a task queue and later executed by the JavaScript Engine.


