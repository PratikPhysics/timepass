# 🐍 Python Basics – One-Page Revision Cheat Sheet

> Covers: Data Types, Variables, Arithmetic, Comparison Operators, Booleans, Statements vs Expressions, Comments, Indentation, and If-Else. 

---

# 1. Python Data Types

| Data Type    | Example               | Description     |
| ------------ | --------------------- | --------------- |
| **int**      | `10`, `-5`            | Whole numbers   |
| **float**    | `3.14`, `2e3`         | Decimal numbers |
| **str**      | `"Hello"`             | Text            |
| **bool**     | `True`, `False`       | Logical values  |
| **datetime** | `2020-08-01 12:23:54` | Date & Time     |

```python
a = 10
b = 3.14
name = "Pratik"
is_student = True
```

---

# 2. Integers vs Floats

| Integer | Float          |
| ------- | -------------- |
| `5`     | `5.0`          |
| `-20`   | `-20.8`        |
| `1000`  | `4E2` (=400.0) |

```python
type(5)      # int
type(5.0)    # float
```

Scientific notation:

```python
4E6      # 4000000.0
6.22E23
```

---

# 3. Variables

A variable stores data.

```python
x = 5
y = 6.4
name = "Python"
```

Check datatype

```python
type(x)
```

Memory address

```python
id(x)
hex(id(x))
```

Variables can change datatype anytime.

```python
x = 5
x = "Hello"
x = True
```

---

# 4. Arithmetic Operators

| Operator | Meaning        | Example     |
| -------- | -------------- | ----------- |
| `+`      | Addition       | `2+3 = 5`   |
| `-`      | Subtraction    | `5-2 = 3`   |
| `*`      | Multiplication | `4*3 = 12`  |
| `/`      | Division       | `5/2 = 2.5` |
| `//`     | Floor Division | `5//2 = 2`  |
| `%`      | Modulus        | `5%2 = 1`   |
| `**`     | Power          | `2**3 = 8`  |

Example

```python
x = 5
y = 2

print(x+y)
print(x-y)
print(x*y)
print(x/y)
print(x//y)
print(x%y)
print(x**y)
```

---

# 5. Floor Division

Returns the **largest integer less than or equal** to the result.

```python
7//2
```

Output

```
3
```

Not

```
3.5
```

---

# 6. Order of Operations (BODMAS)

```python
2 + 10 * 10 + 3
```

Output

```
105
```

Using brackets

```python
2 + 10*(10+3)
```

Output

```
132
```

---

# 7. Variable Naming Rules

✅ Allowed

```python
age
_age
student1
machine_learning
```

❌ Not Allowed

```python
1age
my name
price$
```

Rules

* Start with letter or `_`
* Numbers allowed after first character
* No spaces
* No special symbols
* Case Sensitive

```python
Age
age
AGE
```

All are different variables.

Avoid built-in names

```python
list
str
print
```

---

# 8. Boolean Values

Only two values

```python
True
False
```

```python
flag = True
type(flag)
```

Output

```
bool
```

---

# 9. Comparison Operators

| Operator | Meaning            |
| -------- | ------------------ |
| `==`     | Equal              |
| `!=`     | Not Equal          |
| `>`      | Greater Than       |
| `<`      | Less Than          |
| `>=`     | Greater Than Equal |
| `<=`     | Less Than Equal    |

Examples

```python
2==2
True

2!=3
True

5>3
True

3<2
False

5>=5
True

2<=4
True
```

Remember

```python
=
```

Assignment

```python
==
```

Comparison

---

# 10. Statements vs Expressions

### Statement

Instruction executed by Python.

```python
x = 5
import pandas
if x>2:
```

### Expression

Produces a value.

```python
2+3
len("Hello")
x+5
```

Expressions can appear on the right side of assignments. 

---

# 11. Comments

Single line

```python
# This is a comment
```

Multi-line

```python
"""
Multiple
line
comment
"""
```

Comments improve readability and are ignored by Python. 

---

# 12. Indentation

Python uses indentation (spaces/tabs) to define blocks of code.

```python
if x > 10:
    print("Big")
```

Incorrect indentation causes errors. 

---

# 13. If–Elif–Else

Syntax

```python
if condition:
    statement

elif condition:
    statement

else:
    statement
```

Example

```python
marks = 75

if marks >= 90:
    print("A")

elif marks >= 60:
    print("B")

else:
    print("C")
```

---

# 14. Truthy & Falsy

Falsy values

```python
False
None
0
0.0
''
[]
{}
()
```

Everything else is generally **Truthy**.

Example

```python
if []:
    print("True")
else:
    print("False")
```

Output

```
False
```

```python
if [1]:
    print("True")
```

Output

```
True
```



---

# 15. Most Important Built-in Functions

```python
print()
type()
len()
id()
hex()
```

Examples

```python
print("Hello")
type(10)
len("Python")
id(x)
hex(id(x))
```

---

# 🎯 Exam Quick Recall

✅ Data Types → `int`, `float`, `str`, `bool`, `datetime`

✅ Operators → `+ - * / // % **`

✅ Comparison → `== != > < >= <=`

✅ Assignment → `=`

✅ Comparison → `==`

✅ Check datatype → `type()`

✅ Print → `print()`

✅ Memory address → `id()`

✅ Scientific notation → `4E6`

✅ Floor Division → `//`

✅ Power → `**`

✅ Modulus → `%`

✅ Comments → `#`

✅ Boolean values → `True`, `False`

✅ Conditional statements → `if`, `elif`, `else`

✅ Falsy values → `False`, `None`, `0`, `0.0`, `''`, `[]`, `{}`, `()`
