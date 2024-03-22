# Strings

Strings are a sequence of characters. They are used to represent text-based information.

## Creating Strings

Strings can be created by using single quotes (`'`), double quotes (`"`).

```js
let single_quote_string = 'This is a string'
let double_quote_string = "This is also a string"
let 
```

## Multiline Strings

Multiline strings can be created by using three single quotes (`'''`) or three double quotes (`"""`).

```js
let multiline_string = """
This is a multiline string
"""

let multiline_string = '''
This is a multiline string
'''
```

## String are arrays

Strings are arrays of characters. This means that you can access the characters of a string by using the array syntax.

```js
let string = "Hello World"

print(string[0]) # H
print(string[2]) # l
```

## String length

```js
let string = "Hello World"
string.length() // 11
```

## String concatenation

Strings can be concatenated by using the `+` operator.

```js
let string1 = "Hello"
let string2 = "World"

string1 + " " + string2 // Hello World
```

## Casting

Strings can be casted from other types.

```js
let integer = str(8) // "8"
let float = str(8.0) // "8.0"
let boolean = str(true) // "true"
```

## Escape characters

Escape characters are used to insert characters that are not allowed in a string like `"`.

```js
let string = "Hello \"World\"" // Hello "World"
```

if you want to insert a backslash, you need to escape it.

```js
let string = "Hello \\World\\" // Hello \World\
```

common escape characters:

| Escape character | Description |
| --- | --- |
| `\\` | Backslash |
| `\'` | Single quote |
| `\"` | Double quote |
| `\n` | Newline |
| `\t` | Tab |
| `\b` | Backspace |
| `\r` | Carriage return |
| `\f` | Form feed |
| `\ooo` | Octal value |
| `\xhh` | Hex value |