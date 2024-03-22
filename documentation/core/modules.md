# Modules

Modules serve as a means to structure and organize code, residing in separate files that can be imported into your program. Upon importing a module, its code executes, typically just once throughout the entire program execution.

## Creating a Module

```js
// my_module.qk

export let x = 10
export const y = 20

export function hello()
  print("Hello")
end

export function goodbye()
  print("Goodbye")
end

// Default export
exports {
  test: 30,
  z: x + y,
  j: x
}

// main.qk
import my_module as m
m // { x: 10, y: 20, hello: [Function], goodbye: [Function], test: 30, z: 30, j: 10 }
```

The default export typically encompasses all exports of the module as an object. However, it's also possible to export a single value. Both `export` and `exports` can be employed to export values. Eventually, both approaches will be amalgamated into the default export.

## Importing a Module

```js
import my_module

hello()
```

Here the namespace of the module will be included in the current scope.

## Importing a Module with a Different Name

```js
import my_module as m

m.hello()
```

Here the namespace of the module will be included in the current scope with a different name.

## Importing a Module with Specific Functions

```js
import my_module (hello)

hello() // Hello
goodbye() // Error undefined
```

Here only the specified functions or attribute will be included in the current scope.

```js
import my_module (hello, goodbye)

hello() // Hello
goodbye() // Goodbye
test // Error undefined
```

Here only the specified functions or attribute will be included in the current scope.

## Importing a Module with Specific Functions with Different Names

```js
import my_module (hello as h, goodbye as g)

h()
g()
```
