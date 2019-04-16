# Execution Context
Simply put, an execution context is an abstract concept of an environment where the Javascript code is evaluated and executed. Whenever any code is run in JavaScript, it’s run inside an execution context. <sup>[1](#executionContext)</sup>

Every time a funciton is called, a new execution context is created and pushed to the call stack.

However, inside the JavaScript interpreter, every time an execution context is created, it has 2 stages:

1. Creation (when the function is called, but before it executes and code)
    * Create the scope chain
    * Creates variables, functions, arguments passed to your function, and [`arguments`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments)
    * Determines the value of `this`

2. Activation/Code execution
    * Assign values, references to functions and execute code

<a name="executionContext">1. https://blog.bitsrc.io/understanding-execution-context-and-execution-stack-in-javascript-1c9ea8642dd0</a>