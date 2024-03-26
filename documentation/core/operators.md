# Operators

## Arithmetic Operators

| Operator | Description | Example |
| -------- | ----------- | ------- |
| + | Addition | 1 + 1 |
| - | Subtraction | 1 - 1 |
| * | Multiplication | 1 * 1 |
| / | Division | 1 / 1 |
| % | Modulus | 1 % 1 |
| ** | Exponentiation | 1 ** 1 |

To get the floor division of two numbers, use the `math.floor` function.
  
```python
import math

x = 3
y = 2

print(math.floor(x / y)) // 1
```

## Assignment Operators

| Operator | Description | Example |
| -------- | ----------- | ------- |
| = | Assign value | x = 1 |
| += | Add and assign | x += 1 |
| -= | Subtract and assign | x -= 1 |
| *= | Multiply and assign | x *= 1 |
| /= | Divide and assign | x /= 1 |
| %= | Modulus and assign | x %= 1 |
| **= | Exponentiation and assign | x **= 1 |
| &= | Bitwise AND and assign | x &= 1 |
| \|= | Bitwise OR and assign | x \|= 1 |
| ^= | Bitwise XOR and assign | x ^= 1 |
| >>= | Bitwise right shift and assign | x >>= 1 |
| <<= | Bitwise left shift and assign | x <<= 1 |
| ++ | Post Increment | x++ |
| -- | Post Decrement | x-- |
| ++ | Pre Increment | ++x |
| -- | Pre Decrement | --x |

Pre Increment will increment the value of `x` before using it in the expression. Post Increment will increment the value of `x` after using it in the expression. The same applies to Pre Decrement and Post Decrement.

## Comparison Operators

| Operator | Description | Example |
| -------- | ----------- | ------- |
| == | Equal | 1 == 1 |
| != | Not equal | 1 != 1 |
| > | Greater than | 1 > 1 |
| < | Less than | 1 < 1 |
| >= | Greater than or equal to | 1 >= 1 |
| <= | Less than or equal to | 1 <= 1 |

## Logical Operators

| Operator | Description | Example |
| -------- | ----------- | ------- |
| && | Logical AND | 1 && 1 |
| \|\| | Logical OR | 1 \|\| 1 |
| ! | Logical NOT | !1 |

## Identity Operators

| Operator | Description | Example |
| -------- | ----------- | ------- |
| is | Returns true if both variables are the same object | x is y |

## Membership Operators

| Operator | Description | Example |
| -------- | ----------- | ------- |
| in | Returns true if a sequence with the specified value is present in the object | x in y |

## Bitwise Operators

| Operator | Description | Example |
| -------- | ----------- | ------- |
| & | AND | 1 & 1 |
| \| | OR | 1 \| 1 |
| ^ | XOR | 1 ^ 1 |
| ~ | NOT | ~1 |
| << | Zero fill left shift | 1 << 1 |
| >> | Signed right shift | 1 >> 1 |

## Priority

| Operator | Description |
| -------- | ----------- |
| () | Parentheses |
| ** | Exponentiation |
| +x, -x, ~x | Unary plus, Unary minus, Bitwise NOT |
| *, /, //, % | Multiplication, Division, Floor division, Modulus |
| +, - | Addition, Subtraction |
| <<, >> | Bitwise shift operators |
| & | Bitwise AND |
| ^ | Bitwise XOR |
| \| | Bitwise OR |
| ==, !=, >, >=, <, <=, is, in | Comparisons, Identity, Membership |
| !x | Boolean NOT |
| x && y | Boolean AND |
| x \|\| y | Boolean OR |
