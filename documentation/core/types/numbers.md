# Numbers

## Integers

Integers are whole numbers. They can be positive or negative.

```js
let integer = 8
let integer = -8
```

## Floats

Floats are numbers with a decimal point. They can also be positive or negative.

```js	
let float = 8.0
let float = -8.0
```

## Casting

Numbers can be casted to other types. if you cast a float to an integer, the decimal part will be truncated. but in the memory, the number will be stored as a float for all numbers.

```js
let integer = 8
let float = 8.0

let integer_from_float = int(float) // 8
let float_from_integer = float(integer) // 8.0
```
