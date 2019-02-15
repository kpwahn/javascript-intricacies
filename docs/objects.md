# Objects

## In JavaScript, almost everything is an object
All JavaScript values, except for [primatives](primatives.md), are objects (The inverse is also true).

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

## Ways to define/create objects

1. You can define (and create) a JavaScript object with an [object literal](./object-literal.md):

2. You can define (and create) a JavaScript object with the keyword [`new`](./new-operator.md). You do this by defining a [`class`](./classes.md) or [object constructor function](./object-constructor-function.md). Then you can instantiate  objects of the defined type. 

    * Read more about the [object constructor function](./object-constructor-function.md) for info on why I think you should use the [`class`](./classes.md) syntax instead.

3. You can create a JavaScript object with Object.create();

