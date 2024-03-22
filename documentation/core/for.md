# For

For is a loop that iterates over a list of values.

```js
for let i = 0; i < 10; i++:
  print(i)
end
```

## For .. Else

For loops can have an else block that is executed when the loop is finished. Only executed if the loop is not broken and have at least one iteration.

```js
for let i = 0; i < 10; i++:
  print(i)
else:
  print("Done")
end
// 0
// 1
// ...
// Done
```

## For .. In

For in is used to iterate over the keys of an object.

```js
for let key in {a: 1, b: 2}:
  print(key)
end
// a
// b
```

```js
for let key in [1, 2, 3]:
  print(key)
end
// 0
// 1
// 2
```

```js
for let key in "Hello World":
  print(key)
end
// H
// e
// l
// ...
```

## Break

Break is used to exit a loop.

```js
for let i = 0; i < 10; i++:
  print(i)
  break
end
// 0
```

## Continue

Continue is used to skip the rest of the loop and continue to the next iteration.

```js
for let i = 0; i < 10; i++:
  print(i)
  continue
  print("World")
end
// 0
// 1
// ...
```
