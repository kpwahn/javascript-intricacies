# JavaScript Object Constructors <sup>[1](#JavaScriptObjectConstructors)</sup>

```javaScript
function Person(first, last, age, eye) {
    this.firstName = first;
    this.lastName = last;
    this.age = age;
    this.eyeColor = eye;
}
```

> It is considered good practice to name constructor functions with an upper-case first letter.

In the example above, function Person() is an object constructor function.

Objects of the same type are created by calling the constructor function with the new keyword:

```javaScript
var myFather = new Person("John", "Doe", 50, "blue");
var myMother = new Person("Sally", "Rally", 48, "green");
```

<a name="JavaScriptObjectConstructors">1. https://www.w3schools.com/js/js_object_constructors.asp</a>