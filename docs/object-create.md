# `Object.create`

The Object.create() method creates a new object, using an existing object as the prototype of the newly created object.

```javaScript
const person = {
  isHuman: false,
  printIntroduction: function () {
    console.log(`My name is ${this.name}. Am I human? ${this.isHuman}`);
  }
};

// This creates an empty object that inherits from person
const me = Object.create(person);

console.log(me);

me.name = "Matthew"; // "name" is a property set on "me", but not on "person"
me.isHuman = true; // inherited properties can be overwritten

me.printIntroduction();
```