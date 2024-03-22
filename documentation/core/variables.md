# Variables

Variables are defined with the keyword `let` and are valid only in their execution block and their children, their type can be modified during execution.

## Variables name

Variables name can contain letters, numbers and underscores (`_`), they can't start with a number.

## Case Sensitive

Variables are case sensitive, `variable_name` and `Variable_name` are different variables.

```js
let variable_name = VALUE
let Variable_name = VALUE // Different variable
```

## Creating Variables

```js
let variable_name = VALUE

let first_name = "John"
```

## Modifying Variables

```js
let variable_name = VALUE
variable_name = NEW_VALUE

let first_name = "John"
first_name = "Jane"
```

## Multiple Variables

Multiple variables can be created at the same time.

```js
let variable_name1, variable_name2, variable_name3 = VALUE // Multiple variables with the same value
let variable_name1, variable_name2, variable_name3 = VALUE1, VALUE2, VALUE3 // Multiple variables with different values

let first_name, last_name = "John", "Doe"

first_name, last_name = "John" // Multiple variables with the same value

first_name, last_name" = Jane", "Doe" // Multiple variables with different values


```

## Variable References

Variables are reference by default, to create a copy of a variable, use the function `copy()`.

```js
let variable_name = VALUE
let variable_copy = copy(variable_name)
```

## Global Variables

Variables are defined in current execution block and their children.

## Deleting Variables

Variables can be deleted with the keyword `delete`.

```js
let variable_name = VALUE
delete variable_name
```
