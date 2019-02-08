# `new` operator <sup>[1](#new)</sup>

The new operator lets developers create an instance of a [user-defined object type](./object-constructor-funciton.md) or of one of the <a src="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects">built-in object types</a> that has a constructor function. The new keyword does the following things:

1. Creates a blank, plain JavaScript object;
2. Links (sets the constructor of) this object to another object;
3. Passes the newly created object from Step 1 as the this context;
4. Returns this if the function doesn't return its own object.

```javaScript
function Car(make, model, year) {
  this.make = make;
  this.model = model;
  this.year = year;
}

var car1 = new Car('Eagle', 'Talon TSi', 1993);

console.log(car1.make);
```

This logs an object. Open it.
Check out the `__proto__`. Look at the constructor. It points to the `Car` function
The context for `this` is now our new `car1` object. So when we do `this.make = make` it's updating our `car1` object.
Nothing is returned, so it returns `this`, which is our new object.

<a name="new">1. https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/new</a>
