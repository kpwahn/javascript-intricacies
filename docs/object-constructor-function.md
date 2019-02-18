# JavaScript Object Constructors <sup>[1](#JavaScriptObjectConstructors)</sup>

In JavaScript, constructors are just funcitons that happen to be called with the `new` operator.
*There's really no such thing as "constructor functions," but rather construction calls of functions.*

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

You can also create methods on your object
```javaScript
    function Person(name) {
        this.name = name;
        this.sayHello = function() {
            console.log(`Hello my name is ${this.name}`);
        };
    }

    let kendall = new Person('kendall');
    kendall.sayHello();
```

Buttttttt you might not want to. If you `console.log(kendall)` you'll notice that the `sayHello` method is associated with `kendall`

If you were to create another person
```javaScript
    let sally = new Person('sally');
    console.log(sally);
```
that instance would also have it's own `sayHello` method that is exactly the same as `kendall`'s.

To gain some efficiency (space) you want to declare the method on the prototype
```javaScript
    function Person(name) {
        this.name = name;
    }

    Person.prototype.sayHello = function() {
        console.log(`Hello my name is ${this.name}`);
    };
```

Now when you create a new person, it will be able to `sayHello`, but that functionality won't polute each instance of the Person object. Note that [class]('./classes.md) does this for you for free! #syntaticsugar

<a name="JavaScriptObjectConstructors">1. https://www.w3schools.com/js/js_object_constructors.asp</a>