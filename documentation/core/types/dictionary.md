# Dictionary

Dictionary is a collection of key-value pairs. The key can be a string or a number. The value can be any type and mutable, duplicates are not allowed and the dictionarry is ordered by first created.

## Create dictionary

```js
// Dictionary
let dictionary_var = {"key1": 2, 10: "Hello"} // key can be string or number
```

## Get dictionary element

```js
let dictionary_var = {"key1": 2, 10: "Hello"}
dictionary_var["key1"] // 2
dictionary_var[10] // "Hello"
```

## Set dictionary element

```js
let dictionary_var = {"key1": 2, 10: "Hello"}
dictionary_var["key1"] = 10
dictionary_var[10] = "World"

dictionary_var // {"key1": 10, 10: "World"}
```

## Get dictionary length

```js
let dictionary_var = {"key1": 2, 10: "Hello"}
dictionary_var.length() // 2
```

## Remove element from dictionary at key

```js
let dictionary_var = {"key1": 2, 10: "Hello"}
dictionary_var.remove("key1")

dictionary_var // {10: "Hello"}
```

## Get dictionary keys

```js
let dictionary_var = {"key1": 2, 10: "Hello"}
dictionary_var.keys() // ["key1", 10] as array
```

## Get dictionary values

```js
let dictionary_var = {"key1": 2, 10: "Hello"}
dictionary_var.values() // [2, "Hello"] as array
```

## Check if key is in dictionary

```js
let dictionary_var = {"key1": 2, 10: "Hello"}

// Directly
"key1" in dictionary_var // true
10 in dictionary_var // true
"key2" in dictionary_var // false

// Using keys method
"key1" in dictionary_var.keys() // true
10 in dictionary_var.keys() // true
"key2" in dictionary_var.keys() // false
```

## Check if value is in dictionary

```js
let dictionary_var = {"key1": 2, 10: "Hello"}
"Hello" in dictionary_var.values() // true
2 in dictionary_var.values() // true
"World" in dictionary_var.values() // false
```


## Loop over dictionary

```js
// Loop over dictionary
let dictionary_var = {"key1": 2, 10: "Hello"}
for let key, value in dictionary_var
    print(key, value, dictionary_var[key])
end
// key1 2 2
// 10 Hello Hello

// Loop over dictionary keys
for let key in dictionary_var
    print(key, dictionary_var[key])
end
// key1 2
// 10 Hello
```

## Nested dictionary

```js
let dictionary_var = {"key1": 2, 10: {"key2": 3, 11: "World"}}
dictionary_var[10]["key2"] // 3
```
