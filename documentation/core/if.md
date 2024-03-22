# If

Execution flow is the control if instructions are executed or not, they are a boolean condition inside it.

```js
let a = 1
if a == 1:
    print("Hello")
end
// Hello
```

## If only

```js
if true:
    print("Hello")
end
// Hello

if false:
    print("Hello")
end
//
```

## If .. Else

```js
if true:
    print("Hello")
} else {
    print("World")
}
// Hello

if false:
    print("Hello")
} else {
    print("World")
}
// World
```

## If .. Elif

```js
if true:
    print("Hello")
elseif false:
    print("World")
end
// Hello

if false:
    print("Hello")
elseif true:
    print("World")
end
// World

if false:
    print("Hello")
elseif false:
    print("World")
end
//
```

## If .. Elif .. Else

```js
if true:
    print("Hello")
elseif false:
    print("World")
else:
    print("!")
end
// Hello

if false:
    print("Hello")
elseif true:
    print("World")
else:
    print("!")
end
// World

if false:
    print("Hello")
elseif false:
    print("World")
else:
    print("!")
end
// !
```
