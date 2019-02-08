# JavaScript Object Constructors <sup>[1](#JavaScriptObjectConstructors)</sup>

```javaScript
function Person(first, last, age, eye) {
    this.firstName = first;
    this.lastName = last;
    this.age = age;
    this.eyeColor = eye;
}
```
In the example above, function Person() is an object constructor function.

Objects of the same type are created by calling the constructor function with the new keyword:

```javaScript
    var myFather = new Person("John", "Doe", 50, "blue");
    var myMother = new Person("Sally", "Rally", 48, "green");
```

> It is considered good practice to name constructor functions with an upper-case first letter.

<a name="JavaScriptObjectConstructors">1 - JavaScript Object Constructors - W3 schools</a>