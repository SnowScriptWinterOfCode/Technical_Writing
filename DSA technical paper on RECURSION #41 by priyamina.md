## <h1>Recursion in Data Structures and Algorithms</h1>

### <h2> 1. What is Recursion?</h2>

**Definition:**
Recursion is a programming concept where a function calls itself in its own definition. It is a powerful technique used in algorithms to break down a problem into smaller sub-problems of the same type.

**Key Components:**
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/1573a4a4-2ba8-4951-a21e-61704b453fe2)

- **Base Condition:** A recursive function must have a base condition to stop the recursion. It defines the simplest form of the problem that doesn't require further recursion.
  
- **Stack Overflow:** Without proper base conditions or termination criteria, recursion can lead to a stack overflow, causing the program to crash. It's essential to ensure that the recursion eventually reaches a base case.
  ![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/884d79bb-566f-4a28-b8e1-429cf2063b42)


- **Recursion Tree:** Visualizing recursive calls as a tree structure helps in understanding the flow of the recursive algorithm. Each node in the tree represents a recursive call.

### <h2>2. Examples: Basic Recursion Problems</h2>

#### Example 1: Factorial Calculation
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/d573b824-22d8-4a52-8a2f-4653cc41237c)

```python
def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n-1)
```

#### Example 2: Fibonacci Sequence
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/a5653c0d-1343-4fdf-a862-1946c5dd5314)
```python
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)
```

### <h2>3. Backtracking</h2>

**Definition:**
Backtracking is an algorithmic technique that uses recursion to systematically search for a solution to a problem. If the current solution is not viable, the algorithm backtracks to the previous step and explores other possibilities.

**Example: N-Queens Problem**
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/b63ff631-7906-450f-a398-b03ff355ba50)

```python
def is_safe(board, row, col, n):
    # Check if a queen can be placed in a given position
    # ...

def solve_n_queens(board, row, n):
    if row == n:
        # Base case: All queens are placed successfully
        # Process the solution or store it
    else:
        for col in range(n):
            if is_safe(board, row, col, n):
                # Place queen and move to the next row
                board[row][col] = 1
                solve_n_queens(board, row + 1, n)
                # Backtrack: Remove the queen if the current placement doesn't lead to a solution
                board[row][col] = 0
```

### <h2> 4. Types of Recursion: Parameterized and Functional Recursion</h2>

#### Parameterized Recursion
In parameterized recursion, the recursive function takes additional parameters that help in solving sub-problems.

**Example: Binary Search**
```python
def binary_search(arr, low, high, target):
    if low <= high:
        mid = (low + high) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            return binary_search(arr, mid + 1, high, target)
        else:
            return binary_search(arr, low, mid - 1, target)
    else:
        return -1
```

#### Functional Recursion
In functional recursion, the recursive function returns a modified version of itself.

**Example: Reverse a List**
```python
def reverse_list(lst):
    if not lst:
        return []
    else:
        return reverse_list(lst[1:]) + [lst[0]]
```

### <h2>5. Multiple Recursion Calls with Example</h2>

**Definition:**
Multiple recursion calls occur when a recursive function makes more than one recursive call within its body.

**Example: Merge Sort**
![image](https://github.com/SnowScriptWinterOfCode/Technical_Writing/assets/103628960/b50c881b-b5ba-4e8a-bc70-2e3e4b87b517)

```python
def merge_sort(arr):
    if len(arr) > 1:
        mid = len(arr) // 2
        left_half = arr[:mid]
        right_half = arr[mid:]

        merge_sort(left_half)
        merge_sort(right_half)

        merge(arr, left_half, right_half)
```

In conclusion, recursion is a fundamental concept in computer science and programming, providing an elegant way to solve complex problems by breaking them down into simpler sub-problems. Understanding recursion is crucial for mastering algorithms and data structures, and it opens the door to various problem-solving techniques such as backtracking.
