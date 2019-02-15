# Pass by Value

JavaScript is always pass by value. Period.

Javascript is always pass by value, but when a variable refers to an object (including arrays), the "value" is a reference to the object.
Changing the value of a variable never changes the underlying primitive or object, it just points the variable to a new primitive or object.
However, changing a property of an object referenced by a variable does change the underlying object.

When you assign an object (i.e. a reference) from one variable to another, the value stored in the variable is also copied into the location of the new variable. The difference is that the values stored in both variables now are the address of the actual object stored in the heap. As the result, both variables are pointing to the same object. - http://www.javascripttutorial.net/javascript-primitive-vs-reference-values/

["Arguments are passes to function by *value*"](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions)


- https://stackoverflow.com/questions/7744611/pass-variables-by-reference-in-javascript
- https://stackoverflow.com/questions/373419/whats-the-difference-between-passing-by-reference-vs-passing-by-value