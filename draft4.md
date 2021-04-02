# Design Patterns

_"Design patterns are reusable solutions to commonly occuring problems"_

https://www.toptal.com/javascript/comprehensive-guide-javascript-design-patterns

I think that you will become a effective/efficient coder if you can quickly use a design pattern for a problem at hand.

### What is anti-patterns?
Anti patterns are bad practices and something to be avoided.

Examples of anti-patterns in Javascript
1. Modifying Object class prototype because almost all inherit from Object. A change in the Object will be inherited by all that used Object
1. Modifying Objects that you don't own

### Categories of design patterns

1. Creational
1. Structural
1. Behavioral

### Creational
Deals with creation of objects

1. Constuctor pattern - usually uses the _new_ keyword
```
function Person(name, age) {
  this.name = name
  this.age = age
}

// Constructor pattern
const p1 = new Person("tom", 18)

// Will add to the Person prototype without being created on
// every instance of he Person object
Person.prototype.greet = function() {
  console.log('Hello', this.name)
}
```

2. Module pattern
A pattern to scope variables within the module or a closure

3. Revealing Module Pattern
What ever is the return function or variables will be accessible to the public but private variables are innaccessible from the outside.

4. Singleton
Only one instance of the class should exist. If in case it is already defined then nothing will happen.

5. Factory/Abstract Factory Method
Think of it as function that allows you to create different types of object (e.g CreateCar() can intanstiate a sedan, suv, van)
