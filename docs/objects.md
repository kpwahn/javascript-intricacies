# Objects

## In JavaScript, almost everything is an object
All JavaScript values, except for [primatives](primatives.md), are objects.

An object is a collection of related data and/or functionality (which usually consists of several variables and functions — which are called properties and methods when they are inside objects.

Objects look like this:
```javascript
    {
        name: "John",                     // property
        sayHello: function() {            // method
            console.log('Saying hello!');
        }
    }
```

You can define (and create) a JavaScript object with an [object literal](./object-literal.md):
```javascript
    var person = {
        name: "John"
    };
```

You can define (and create) a JavaScript object with the keyword `new`.

You can define an [object constructor function](./object-constructor-function.md), and then create objects for the constructed type.

You can create a JavaScript object with Object.create();

