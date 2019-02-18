# Object Literals (also called object initializers)

This is the easiest way to create a JavaScript Object.

Using an object literal, you both define and create an object in one statement.

An object literal is a list of name:value pairs (like age: 30) inside curly braces {}.

The following example creates a new JavaScript object with two properties:

```javascript
let person = {
    age: 30,
    name: "John",
    sayHello: function() {
        console.log(`hello my name is ${this.name}`);
    }
}
```

Objects are created as if a call to [new](./new-operator.md) Object() were made; that is, objects made from object literal expressions are instances of Object.