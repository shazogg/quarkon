# Booleans

Boolean is a data type that can have one of two values: `true` or `false`.

```js
let boolean = true
boolean = false
```

## Boolean operators

Boolean operators are used to compare values and return a boolean value.

```js
let boolean = true

boolean == true // true
boolean == false // false

boolean != true // false
boolean != false // true

let number = 1

number == 1 // true
number == 2 // false
```

## Casting

To cast a value to a boolean, use the `bool` function.

```js
let boolean = bool(true) // true
boolean = bool(123) // true
boolean = bool("Hello") // true
boolean = bool(["Hello"]) // true


boolean = bool(false) // false
boolean = bool(0) // false
boolean = bool("") // false
boolean = bool(()) // false
boolean = bool([]) // false
boolean = bool({}) // false
boolean = bool(undefined) // false
boolean = bool(null) // false
```
