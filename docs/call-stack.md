# The call stack <sup>[1](#callStack)</sup>

A call [stack](https://en.wikipedia.org/wiki/Stack_(abstract_data_type)) is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

This code (which really does nothing):

```javaScript
function x() {
    function y() {
        function z() {
        };
        z();
    };
    y();
};

x();
```

Looks like this to the call stack:
```
                            z
                    y       y       y
            x       x       x       x       x
    global  global  global  global  global  global  global  
```
Not the call stack is initially empty.

When javascript (the browser, or node) starts running your code, it creates and enters a global execution context (and global memory) by default and pushes that context to your call stack. 

As functions are called, they (and their [execution context](./execution-context.md)) are pushed to the call stack.

<a name="callStack">1. https://developer.mozilla.org/en-US/docs/Glossary/Call_stack</a>
