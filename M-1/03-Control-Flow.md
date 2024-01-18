# Control Flow

## If Statements:

1.  **Basic Conditions:**

    - Equals: `a == b`
    - Not Equals: `a != b`
    - Less than: `a < b`
    - Less than or equal to: `a <= b`
    - Greater than: `a > b`
    - Greater than or equal to: `a >= b`

2.  **If Statements:**

    - Basic syntax: `if condition:`
    - Example:

      ```python
      a = 33
      b = 200
      if b > a:
          print("b is greater than a")
      ```

3.  **Elif (Else If):**

    - Used when the previous conditions are not true.
    - Example:

      ```python
      a = 33
      b = 33
      if b > a:
          print("b is greater than a")
      elif a == b:
          print("a and b are equal")
      ```

4.  **Else:**

    - Catches anything not caught by preceding conditions.
    - Example:

      ```python
      a = 200
      b = 33
      if b > a:
          print("b is greater than a")
      elif a == b:
          print("a and b are equal")
      else:
          print("a is greater than b")
      ```

5.  **Short Hand `if`:**

    - If you have only one statement, you can put it on the same line.
    - Example: `if a > b: print("a is greater than b")`

6.  **Short Hand `if ... else`:**

    - One line if-else statement using the ternary operator.
    - Example: `print("A") if a > b else print("B")`

7.  **Logical Operators:**

    #### **`and`**

    - Combines conditional statements.
    - Example: `if a > b and c > a: print("Both conditions are True")`

    #### `or`

    - Combines conditional statements.
    - Example: `if a > b or a > c: print("At least one of the conditions is True")`

    #### `not`

    - Reverses the result of the conditional statement.
    - Example: `if not a > b: print("a is NOT greater than b")`

8.  **Nested If Statements:**

    - You can have if statements inside if statements.
    - Example:

      ```python
      x = 41
      if x > 10:
          print("Above ten,")
          if x > 20:
              print("and also above 20!")
          else:
              print("but not above 20.")
      ```

9.  **The `pass` Statement:**

    - Used to avoid errors in empty if statements.
    - Example:

      ```python
      if some_condition:
          pass
      ```

---

## Loops

### For Loops:

#### 1. **Understanding For Loops:**

- **Definition:** For loops are used for iterating over a sequence (list, tuple, etc.).
- **Functionality:** Executes a set of statements for each item in the sequence.
- **Example:**

  ```python
  colors = ["red", "green", "blue"]
  for color in colors:
      print("Color:", color)
  # Output: Color: red
  #         Color: green
  #         Color: blue
  ```

#### 2. **Using the `break` Statement:**

- **Purpose:** Stops the loop before it completes all iterations.
- **Example:**

  ```python
  numbers = [1, 2, 3, 4, 5]
  for num in numbers:
      if num == 3:
          break
      print("Number:", num)
  # Output: Number: 1
  #         Number: 2
  ```

#### 3. **Using the `continue` Statement:**

- **Purpose:** Skips the current iteration and moves to the next.
- **Example:**

  ```python
  fruits = ["apple", "orange", "banana", "cherry"]
  for fruit in fruits:
      if fruit == "banana":
          continue
      print("Fruit:", fruit)
  # Output: Fruit: apple
  #         Fruit: orange
  #         Fruit: cherry
  ```

#### 4. **Else in For Loop:**

- **Purpose:** Specifies code to be executed when the loop is finished.
- **Example:**

  ```python
  for i in range(5):
      print("Index:", i)
  else:
      print("Loop Completed!")
  # Output: Index: 0
  #         Index: 1
  #         Index: 2
  #         Index: 3
  #         Index: 4
  #         Loop Completed!
  ```

#### 5. **Nested Loops:**

- **Purpose:** A loop inside a loop (inner loop for each iteration of the outer loop).
- **Example:**

  ```python
  adjectives = ["bright", "small", "sweet"]
  fruits = ["apple", "grape", "melon"]
  for adj in adjectives:
      for fruit in fruits:
          print(adj, fruit)
  # Output: bright apple
  #         bright grape
  #         bright melon
  #         small apple
  #         small grape
  #         small melon
  #         sweet apple
  #         sweet grape
  #         sweet melon
  ```

#### 6. **The pass Statement:**

- **Purpose:** Used in empty for loops to avoid errors.
- **Example:**

  ```python
  for item in my_list:
      pass
  # No output (pass statement does nothing)
  ```

### While Loop:

- Repeatedly executes a block of code while a condition is true.
- **Example 1:**

  ```python
  i = 1
  while i <= 5:
      print(i)
      i += 1
  # Output: 1 2 3 4 5
  ```

- **Example 2:** using `while`, `break`, `continue`, and `else`.

  ```python
  i = 1
  while i <= 5:
      print(i)
      if i == 3:
          print("Breaking loop at i = 3")
          break
      if i == 2:
          print("Skipping iteration at i = 2")
          i += 1
          continue
      i += 1
  else:
      print("i is no longer less than 6")
  # Output: 1 2 Skipping iteration at i = 2 4 Breaking loop at i = 3
  ```

---
