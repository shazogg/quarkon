# Try ... Catch

Try ... Catch is a way to handle errors in a more controlled way. It is a way to tell the program what to do when an error occurs.

```js
try:
  // code that might throw an error
catch (e):
  // code to handle the error
end
```

```js
try:
  let a = 1 / 0;
catch (e):
  print(e);
end
```

## Try .. Ctach .. Finally

```js
try:
  // code that might throw an error
catch (e):
  // code to handle the error
finally:
  // code that will always run
end
```

```js
try:
  let a = 1 / 0;
catch (e):
  print(e);
finally:
  print("finally");
end
```

## Try .. Ctach .. Else

```js
try:
  // code that might throw an error
catch (e):
  // code to handle the error
else:
  // code that will only run if no error is thrown
end
```

```js
try:
  let a = 1 / 1;
catch (e):
  print(e);
else:
  print("else");
end
```

## Try .. Ctach .. Else .. Finally

```js
try:
  // code that might throw an error
catch (e):
  // code to handle the error
else:
  // code that will only run if no error is thrown
finally:
  // code that will always run
end
```


```js
try:
  let a = 1 / 1;
catch (e):
  print(e);
else:
  print("else");
finally:
  print("finally");
end
```
