# Class

Class is a blueprint for creating objects. It defines the data and behavior of a type.

## Creating a Class

A class is created using the `class` keyword.

```js
class Person
  let name

  function constructor(name)
    this.name = name
  end

  function sayHello()
    print("Hello, my name is " + this.name)
  end
end
```

## Creating an Object

An object is created using the `new` keyword. The object is like a dictionary of properties and methods.

```js
let person = new Person("John")
```

## Accessing Properties

Properties are accessed using the `.` operator.

```js
let person = new Person("John")
person.name = "Jane" // Dont work on classic dictionary
```

## Calling Methods

Methods are called using the `.` operator.

```js
let person = new Person("John")
person.sayHello() // Dont work on classic dictionary
```

## Inheritance

A class can inherit from another class using the `extends` keyword. `super` keyword is used to call the parent class constructor and methods.

```js
class Person
  let name

  function constructor(name)
    this.name = name
  end

  function sayHello()
    print("Hello, my name is " + this.name)
  end
end

class Student extends Person
  let grade

  function constructor(name, grade)
    super(name)
    this.grade = grade
  end

  function sayHello()
    super.sayHello()
    print("I am in grade " + this.grade)
  end
end
```

## Polymorphism

A subclass can override methods of the parent class.

```js
class Person
  let name

  function constructor(name)
    this.name = name
  end

  function sayHello()
    print("Hello, my name is " + this.name)
  end
end

class Student extends Person
  function constructor(name, grade)
    super(name)
    this.grade = grade
  end

  function sayHello()
    print("I am in grade " + this.grade)
  end
end

let person = new Person("John")
let student = new Student("Jane", 5)

person.sayHello() // Hello, my name is John
student.sayHello() // I am in grade 5
```
