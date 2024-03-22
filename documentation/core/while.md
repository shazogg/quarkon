# While

While loops are used to repeat a block of code while a condition is true.

```js
while true
    print("Hello")
end
// prints "Hello" forever
```

## While .. Else

While loops can have an else block that is executed when the condition is false.

```js
i = 0
while i < 3
    print("Hello")
    i++
else
    print("World")
end
// prints "Hello" three times and "World"
```

## Break

Break is used to exit a loop.

```js
while true
    print("Hello")
    break
end
// prints "Hello" once
```

## Continue

Continue is used to skip the rest of the loop and continue to the next iteration.

```js
while true
    print("Hello")
    continue
    print("World")
end
// prints "Hello" forever
```
