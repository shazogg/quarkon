# Modules

Modules are a way to organize your code. They are in another file and can be imported into your program.

## Creating a Module

```js
// my_module.qk

export let x = 10
export const y = 20

export function hello():
  print("Hello")
end

export function goodbye():
  print("Goodbye")
end

exports {
  test: 30,
  z: x + y,
  j: x
}

// main.qk
import my_module as m
m // { x: 10, y: 20, hello: [Function], goodbye: [Function], test: 30, z: 30, j: 10 }
```

## Importing a Module

```js
import my_module

hello()
```

## Importing a Module with a Different Name

```js
import my_module as m

m.hello()
```

## Importing a Module with Specific Functions

```js
import my_module (hello)

hello()
```

```js
import my_module (hello, goodbye)

hello()
goodbye()
```

## Importing a Module with Specific Functions with Different Names

```js
import my_module (hello as h, goodbye as g)

h()
g()
```
