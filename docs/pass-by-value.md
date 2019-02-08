# Pass by Value

JavaScript is always pass by value. Period.

Javascript is always pass by value, but when a variable refers to an object (including arrays), the "value" is a reference to the object.
Changing the value of a variable never changes the underlying primitive or object, it just points the variable to a new primitive or object.
However, changing a property of an object referenced by a variable does change the underlying object.