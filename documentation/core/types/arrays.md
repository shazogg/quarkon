# Arrays

Arrays are ordered and mutable, integer-indexed collections of any data type. Array elements can be accessed using the array index. Duplicate elements are allowed and can contain differents types.

## Create array

```js
let array_var = [4, 5, 6] // Mutable array
```

## Get array element

```js
let array_var = [4, 5, 6]
array_var[0] // 4
```

## Set array element

```js
let array_var = [4, 5, 6]
array_var[0] = 10

array_var // [10, 5, 6]
```

## Get array length

```js
let array_var = [4, 5, 6]
array_var.length() // 3
```

## Remove element from array at index

```js
let array_var = [4, 5, 6]
array_var.remove(1)

array_var // [4, 6]
```

## Negative index

```js
let array_var = [4, 5, 6, 7, 8, 9]
array_var[-1] // 9
array_var[-2] // 8
```

## Index range

```js
let array_var = [4, 5, 6, 7, 8, 9]
array_var[1:3] // [5, 6]
array_var[1:] // [5, 6, 7, 8, 9]
array_var[:3] // [4, 5, 6]
array_var[-4:-2] // [6, 7]
```

## Check if element is in array

```js
let array_var = [4, 5, 6, 7, 8, 9]
array_var.contains(5) // true
array_var.contains(10) // false
```

## Concatenate arrays

```js
let array_var = [4, 5, 6]
let array_var2 = [7, 8, 9]
array_var + array_var2 // [4, 5, 6, 7, 8, 9] not sorted
```

## Loop through array

```js
let array_var = [4, 5, 6]

// Loop through array
for let value in array_var:
    print(value)
end
// 4
// 5
// 6

// Loop through array with index
for let index, value in array_var:
    print(index, value, array_var[index])
end
// 0 4 4
// 1 5 5
// 2 6 6
```

## Nested arrays

```js
let array_var = [4, 5, 6]
let array_var2 = [7, 8, 9]
let array_var3 = [array_var, array_var2] // [[4, 5, 6], [7, 8, 9]]

array_var3[0][1] // 5
```
