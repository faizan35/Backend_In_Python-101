# Functions

### 1. **Function Basics:**

- A function is a block of code that runs when called.
- Parameters (data) can be passed into a function, and it can return data as a result.
- **Example:**

```python
def greet():
    print("Hello, welcome to the function!")

greet()  # Calling the function

# Output: Hello, welcome to the function!
```

### 2. **Creating a Function in Python:**

- Define a function using the **`def`** keyword.
- To call a function, use the function name followed by parentheses.
- **Example:**

```python
def add_numbers(x, y):
    result = x + y
    return result

sum_result = add_numbers(5, 3)
print(sum_result)
# Output: 8
```

### 3. **Function with Arguments:**

- Information passed into functions is called arguments.
- Passing **Alice** as an argument.

- **Example:**

```python
def greet_person(name):
    print("Hello, " + name + "!")

greet_person("Alice")
# Output: Hello, Alice!
```

### 4. **Arbitrary Arguments (`*args`):**

- Use `*` before parameter name for an unknown number of arguments.

- **Example:**

```python
def print_items(*args):
    for item in args:
        print(item)

print_items("apple", "banana", "cherry")

# Output:
# apple
# banana
# cherry
```

### 5\. **Keyword Arguments (`kwargs`):**

- Arguments can be sent with `key = value` syntax.
- Order of arguments does not matter.
- **Example:**

```python
def display_info(name, age):
    print("Name:", name)
    print("Age:", age)

display_info(age=25, name="Bob")

# Output:
# Name: Bob
# Age: 25
```

### 6. **Arbitrary Keyword Arguments (`**kwargs`):\*\*

- Use `**` before parameter name for an unknown number of keyword arguments.
- Function receives a dictionary of arguments.
- **Example:**

```python
def print_details(**kwargs):
    for key, value in kwargs.items():
        print(key + ": " + value)

print_details(fname="John", lname="Doe", age="30")

# Output:
# fname: John
# lname: Doe
# age: 30
```

### 7. **Default Parameter Value:**

- Set default parameter values in function definition.
- If no argument is provided, default value is used.
- **Example:**

```python
def greet_country(country="World"):
    print("Hello from", country)

greet_country("India")
greet_country()  # Uses default value "World"

# Output:
# Hello from India
# Hello from World
```

### 8. **Return Values:**

- Use the `return` statement to make a function return a value.
- **Example:**

```python
def multiply_by_five(x):
    return 5 * x

result = multiply_by_five(4)
print(result)

# Output: 20
```

---

## Lambda Functions:

### 1. **Introduction:**

- Lambda functions are small, anonymous functions in Python.
- They can take any number of arguments but have only one expression.

### 2. **Syntax:**

```python
lambda arguments : expression
```

- Example: Multiply two arguments (`a` and `b`):

```python
x = lambda a, b: a * b
print(x(5, 6))

# Output: 30
```

#### 3. **Multiple Arguments:**

- Lambda functions can handle multiple arguments.
- Example: Summarize three arguments (`a`, `b`, and `c`):

```python
x = lambda a, b, c: a + b + c
print(x(5, 6, 2))

# Output: 13
```

#### 4. **Using Lambda Inside Another Function:**

- Lambda functions are powerful when used inside another function.
- Example: Create a function (`myfunc`) that returns a lambda function:

```python
def myfunc(n):
    return lambda a: a * n

# Double and triple using the same function definition
mydoubler = myfunc(2)
mytripler = myfunc(3)

print(mydoubler(11))  # Output: 22
print(mytripler(11))  # Output: 33
```

#### 5. **Multiple Lambda Functions:**

- The same function definition can be used to create multiple lambda functions.
- Example:

```python
def myfunc(n):
    return lambda a: a * n

mydoubler = myfunc(2)
mytripler = myfunc(3)

print(mydoubler(11))  # Output: 22
print(mytripler(11))  # Output: 33
```

#### 6. **Use Cases for Lambda Functions:**

- Lambda functions are useful for short-term, anonymous functionality.
- Example: Using lambda for a short period:

```python
# Using lambda for a short period
add = lambda x, y: x + y
result = add(3, 4)
print(result)  # Output: 7
```

#### 7. **Summary:**

- Lambda functions are handy for brief operations.
- Especially powerful when used inside other functions.
- Useful for situations where a quick, anonymous function is needed.

---
