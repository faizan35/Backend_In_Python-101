# Python Basics

## Comment

### Single line Comments

```python
# This is a comment
print("Hello, World!")
```

### Multiline Comments

```python
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")
```

## Variables

### Variable Names:

- Variable names can contain letters, numbers, and underscores.
- They cannot start with a number.
- Case-sensitive (`myVar` and `myvar` are different variables).

### Global Variables

- If you use the global keyword, the variable belongs to the **global** scope:

  ```python
  def myfunc():
  global x
  x = "fantastic"

  myfunc()

  print("Python is " + x)
  ```

## Python Data Types:

Python has several data types:

- **Numbers:** Integers (`int`) and Floats (`float`).
- **Strings:** Textual data (`str`).
- **Booleans:** True (`True`) or False (`False`).

### Python Numbers:

```python
x = 5       # int
y = 3.14    # float
z = 1j      # complex
```

### Python Casting:

You can convert one data type to another using casting:

```python
x = int(3.14)
y = float("5.2")
z = str(10)
```

## Python Strings:

Strings are sequences of characters. You can use single (`'`) or double (`"`) quotes:

```python
my_string = "Hello, World!"
```

```python
my_string = 'Hello, World!'
```

## Python Booleans:

Boolean values represent truth or falsehood. They are used in conditions and comparisons:

```python
is_true = True
is_false = False
```

## Python Operators:

Python supports various operators for performing operations:

- **Arithmetic Operators:** `+, -, *, /, %, **`
- **Comparison Operators:** `==, !=, <, >, <=, >=`
- **Logical Operators:** `and, or, not`

```python
a = 5
b = 3

result = (a + b) * 2
is_greater = a > b
logical_result = (a > 0) and (b < 5)
```

---
