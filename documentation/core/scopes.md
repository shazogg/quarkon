# Scopes

Scope is a set of rules that determines the visibility of a variable. It defines where the variable is accessible from.

## Global Scope

Variables declared outside of a function are in the global scope. They are accessible from anywhere in the program.

```js
let a = 1;

function foo():
  print(a);
end

foo(); // prints 1
```

## Local Scope

Variables declared inside of a function are in the local scope. They are only accessible from within the function.

```js
function foo():
  let a = 1;
  print(a);
end

foo(); // prints 1

print(a); // error: a is not defined
```

## Block Scope

Variables declared inside of a block are in the block scope. They are only accessible from within the block.

```js
if (true):
  let a = 1;
  print(a);
end

print(a); // error: a is not defined
```

## Nested Scope

Variables declared in an inner scope are accessible from an outer scope.

```js
function foo():
  let a = 1;
  function bar():
    print(a);
  end
  bar();
end

foo(); // prints 1
```

## Shadowing

Variables in an inner scope can have the same name as variables in an outer scope. This is called shadowing. The inner variable shadows the outer variable.

```js

let a = 1;

function foo():
  let a = 2;
  print(a);
end

foo(); // prints 2
print(a); // prints 1
```
