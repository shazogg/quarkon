# Function

Functions are the main building blocks of a program. They allow the programmer to define a block of code that can be called repeatedly, without needing to copy the code. Functions can be used to perform a specific task, and can be called from anywhere in the program. This allows for code reuse, and makes programs more modular. Argument are required.

## Defining a Function

```js
function function_name(arg1, arg2, ...)
  // Code
end
```

## Calling a Function

```js
function_name(arg1, arg2, ...)
```

## Return

Functions can return a value using the `return` keyword.

```js
function add(a, b)
  return a + b
end

let result = add(1, 2) // 3
```

## Arguments

Functions can take arguments.

```js
function add(a, b)
  return a + b
end

let result = add(1, 2)
```

## Default Arguments

Functions can have default arguments.

```js
function add(a, b = 3)
  return a + b
end

let result = add(1) // 4
```

## Rest Arguments

Functions can take a variable number of arguments using the `...` operator.

```js
function add(...args)
  let result = 0
  for let arg in args
    result += arg
  end
  return result
end

let result = add(1, 2, 3, 4, 5) // 15
```

## Named Arguments

Functions can take named arguments.

```js
function add(a, b)
  return a + b
end

let result = add(b = 1, a = 2) // 3
```

## Anonymous Functions

Functions can be anonymous.

```js
let add = function(a, b)
  return a + b
end

let result = add(1, 2) // 3
```

## Arrow Functions

Functions can be defined using the arrow syntax.
Arrow functions are always anonymous.
Arrow functions do not have their own `this` value, there is no context.

```js
let add = (a, b) => a + b

let result = add(1, 2)
```

## Function Overloading

Functions can be overloaded.

```js
function add(a, b)
  return a + b
end

function add(a, b, c)
  return a + b + c
end

let result1 = add(1, 2) // 3
let result2 = add(1, 2, 3) // 6
```

## Recursion

Functions can call themselves.

```js
function factorial(n)
  if n == 0
    return 1
  end
  return n * factorial(n - 1)
end

let result = factorial(5) // 120
```

Recursion have a limit of 1000 calls. but this can be changed using the `set_stack_limit(int)` function.
