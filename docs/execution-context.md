# Execution Context

Every time a funciton is called, a new execution context is created and pushed to the call stack.

However, inside the JavaScript interpreter, every call to an execution context has 2 stages:

1. Creation (when the function is called, but before it executes and code)
    * Create the scope chain
    * Creates variables, functions, arguments passed to your function, and [`arguments`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments)
    * Determines the value of `this`

2. Activation/Code execution
    * Assign values, references to functions and execute code