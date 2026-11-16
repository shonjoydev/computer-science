# Chapter 2: Recursion and Backtracking

## Contents <!-- omit from toc -->

- [2.1 Introduction](#21-introduction)
- [2.2 What is Recursion?](#22-what-is-recursion)
- [2.3 Why Recursion?](#23-why-recursion)
- [2.4 Format of a Recursive Function](#24-format-of-a-recursive-function)
- [2.5 Recursion and Memory (Visualization)](#25-recursion-and-memory-visualization)
- [2.6 Recursion versus Iteration](#26-recursion-versus-iteration)
- [2.7 Notes on Recursion](#27-notes-on-recursion)
- [2.8 Example Algorithms of Recursion](#28-example-algorithms-of-recursion)
- [2.9 Recursion: Problems \& Solutions](#29-recursion-problems--solutions)
- [2.10 What is Backtracking?](#210-what-is-backtracking)
- [2.11 Example Algorithms of Backtracking](#211-example-algorithms-of-backtracking)
- [2.12 Backtracking: Problems \& Solutions](#212-backtracking-problems--solutions)

---

## 2.1 Introduction

In this chapter, we will look at one of the important topics, **recursion**, which will be used in almost every chapter, and also its relative **backtracking**.

---

## 2.2 What is Recursion?

Any function which calls itself is called **recursive**. A recursive method solves a problem by calling a copy of itself to work on a smaller problem. This is called the **recursion step**. The recursion step can result in many more such recursive calls.

It is important to ensure that the recursion terminates. Each time the function calls itself with a slightly simpler version of the original problem. The sequence of smaller problems must eventually converge on the base case.

---

## 2.3 Why Recursion?

Recursion is a useful technique borrowed from mathematics. Recursive code is generally shorter and easier to write than iterative code. Generally, loops are turned into recursive functions when they are compiled or interpreted.

Recursion is most useful for tasks that can be defined in terms of similar subtasks. For example, sort, search, and traversal problems often have simple recursive solutions.

---

## 2.4 Format of a Recursive Function

A recursive function performs a task in part by calling itself to perform the subtasks. At some point, the function encounters a subtask that it can perform without calling itself. This case, where the function does not recur, is called the **base case**. The case where the function calls itself to perform a subtask is referred to as the **recursive case**.

We can write all recursive functions using the following general format:

```python
if (test_for_base_case):
    return base_case_value
elif (test_for_another_base_case):
    return other_base_case_value
else:
    return (some_work_and_then_a_recursive_call)
```

As an example, consider the **factorial** function: $n!$ is the product of all integers between $n$ and $1$. The definition of recursive factorial is:

- $n! = 1$ if $n = 0$
- $n! = n \times (n-1)!$ if $n > 0$

Here, the problem is determining the value of $n!$, and the subproblem is determining the value of $(n-1)!$. In the recursive case, when $n$ is greater than 1, the function calls itself to determine the value of $(n-1)!$ and multiplies that with $n$. In the base case, when $n$ is 0 or 1, the function simply returns 1.

```python
def Fact(n):
    # Calculates factorial of a positive integer
    if n == 1:
        return 1 # Base case: fact of 1 is 1
    elif n == 0:
        return 1 # Base case: fact of 0 is 1
    else:
        # Recursive case: multiply n by (n-1) factorial
        return n * Fact(n - 1)
```

---

## 2.5 Recursion and Memory (Visualization)

Each recursive call makes a new copy of that method (actually only the variables) in memory. Once a method ends (that is, returns some data), the copy of that returning method is removed from memory. The recursive solutions look simple but visualization and tracing takes time.

For better understanding, let us consider an example function that prints numbers from $1$ to $n$ backward:

```python
def Print_Recursive(n):
    # Print numbers 1 to n backward
    if n == 0:
        return 0 # This is the terminating base case
    else:
        print(n, end=" ") # Print current number
        return Print_Recursive(n - 1) # Recursive call to itself again
```

For this example, if we call the print function with $n=4$, visually our memory assignments may look like:

![TREES show-in-dark](assets/recursion_print_dark.svg#gh-light-mode-only)
![TREES show-in-light](assets/recursion_print_light.svg#gh-dark-mode-only)

Now, let us consider our factorial function. The visualization of factorial function with n=4 will look like:

![TREES show-in-dark](assets/recursion_factorial_dark.svg#gh-light-mode-only)
![TREES show-in-light](assets/recursion_factorial_light.svg#gh-dark-mode-only)

---

## 2.6 Recursion versus Iteration

While discussing recursion, the basic question that comes to mind is: which way is better? iteration or recursion? The answer to this question depends on what we are trying to do. A recursive approach mirrors the problem that we are trying to solve. A recursive approach makes it simpler to solve a problem that may not have the most obvious of answers. However, recursion adds overhead for each recursive call because it requires space on the stack frame.

A comparison of their key differences is summarized below:

| Recursion                                                                                     | Iteration                                                                              |
| :-------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------- |
| Terminates when a base case is reached.                                                       | Terminates when a condition is proven to be false.                                     |
| Each recursive call requires extra space on the stack frame (memory).                         | Each iteration does not require extra space.                                           |
| If we get infinite recursion, the program may run out of memory and result in stack overflow. | An infinite loop could loop forever since there is no extra memory being created.      |
| Solutions to some problems are easier to formulate recursively.                               | Iterative solutions to a problem may not always be as obvious as a recursive solution. |

---

## 2.7 Notes on Recursion

- Recursive algorithms have two types of cases: recursive cases and base cases.
- Every recursive function case must terminate at a base case.
- Generally, iterative solutions are more efficient than recursive solutions due to the overhead of function calls.
- A recursive algorithm can be implemented without recursive function calls using a stack, but it's usually more trouble than its worth. That means any problem that can be solved recursively can also be solved iteratively.
- For some problems, there are no obvious iterative algorithms.
- Some problems are best suited for recursive solutions while others are not.

---

## 2.8 Example Algorithms of Recursion

- Fibonacci Series, Factorial Finding
- Merge Sort, Quick Sort
- Binary Search
- Tree Traversals and many Tree Problems: InOrder, PreOrder, PostOrder
- Graph Traversals: DFS [Depth First Search] and BFS [Breadth First Search]
- Dynamic Programming Examples
- Divide and Conquer Algorithms
- Towers of Hanoi
- Backtracking Algorithms

---

## 2.9 Recursion: Problems & Solutions

This section covers basic recursive problems and their corresponding step-by-step algorithms and implementations.

### 1. Discuss Towers of Hanoi puzzle

The **Towers of Hanoi** is a mathematical puzzle. It consists of three rods (or pegs or towers), and a number of disks of different sizes which can slide onto any rod. The puzzle starts with the disks on one rod in ascending order of size, the smallest at the top, thus making a conical shape. The objective of the puzzle is to move the entire stack to another rod, satisfying the following rules:

- Only one disk may be moved at a time.
- Each move consists of taking the upper disk from one of the rods and sliding it onto another peg, on top of the other disks that may already be present on that peg.
- No disk may be placed on top of a smaller disk.

The greedy recursive algorithm is formulated as follows:

1. Move the top $n-1$ disks from the Source peg to the Auxiliary peg.
2. Move the $n^{th}$ disk from the Source peg to the Destination peg.
3. Move the $n-1$ disks from the Auxiliary peg to the Destination peg.

```python
def TowersOfHanoi(n, frompeg, topeg, auxpeg):
    # If only 1 disk, make the move and return
    if n == 1:
        print(f"Move disk 1 from peg {frompeg} to peg {topeg}")
        return

    # Move top n-1 disks from A to B, using C as auxiliary
    TowersOfHanoi(n - 1, frompeg, auxpeg, topeg)

    # Move remaining disks from A to C
    print(f"Move disk {n} from peg {frompeg} to peg {topeg}")

    # Move n-1 disks from B to C using A as auxiliary
    TowersOfHanoi(n - 1, auxpeg, topeg, frompeg)
```

---

### 2. Given an array, check whether the array is in sorted order with recursion

To check if an array is in sorted order recursively, we compare each element at the tail of the array with its preceding element. If any element is smaller than its predecessor, the array is not sorted; otherwise, we recursively check the subarray of size $n-1$.

```python
def isArrayInSortedOrder(A, n):
    if n == 1:
        return 1 # Base case: an array of size 1 is always sorted

    # Check if current element is smaller than predecessor, else recurse
    return 0 if A[n-1] < A[n-2] else isArrayInSortedOrder(A, n - 1)
```

- **Time Complexity**: $O(n)$ for scanning the array of size $n$.
- **Space Complexity**: $O(n)$ for recursive stack space.

---

## 2.10 What is Backtracking?

**Backtracking** is an improvement of the brute force approach. It systematically searches for a solution to a problem among all available options. In backtracking, we start with one possible option out of many available options and try to solve the problem. If we are able to solve the problem with the selected move, then we print the solution, else we backtrack and select some other option and try to solve it. If none of the options work out, we claim that there is no solution for the problem.

Backtracking is a form of recursion. The usual scenario is that you are faced with a number of options, and you must choose one of these. After you make your choice you will get a new set of options; just what set of options you get depends on what choice you made. This procedure is repeated over and over until you reach a final state.

Backtracking can be thought of as a selective tree/graph traversal method. The tree is a way of representing some initial starting position (the root node) and a final goal state (one of the leaves). Backtracking allows us to deal with situations in which a raw brute-force approach would explode into an impossible number of options to consider. At each node, we eliminate choices that are obviously not possible and proceed to recursively check only those that have potential.

We back up only as far as needed to reach a previous decision point with an as-yet-unexplored alternative. Eventually, more and more of these decision points will have been fully explored, and we will have to backtrack further and further. If we backtrack all the way to our initial state and have explored all alternatives from there, we can conclude the particular problem is unsolvable.

Some basic backtracking objects we can generate include:

- Binary strings: $2^n$ possibilities for $n$-bit strings.
- Permutations: $n!$ possibilities.
- Combinations: $\frac{n!}{r!(n-r)!}$ possibilities.
- General strings: $k$-ary strings of length $n$ ($k^n$ possibilities).

---

## 2.11 Example Algorithms of Backtracking

- Generating all Binary Strings
- Generating $k$-ary Strings
- N-Queens Problem
- The Knapsack Problem
- Generalized Strings
- Hamiltonian Cycles
- Graph Coloring Problem

---

## 2.12 Backtracking: Problems & Solutions

### 3. Generate all the strings of $n$ bits. Assume $A[0 \dots n-1]$ is an array of size $n$

To generate all binary strings of length $n$, we use a backtracking approach. We set each position $n-1$ to $0$ and recurse, and then set it to $1$ and recurse. Once we hit the base case where $n < 1$, we print the accumulated string.

```python
def Binary(n, A=None):
    if A is None:
        A = [0] * n # Assume array A is initialized
    if n < 1:
        print("".join(map(str, A))) # Print the completed binary string
    else:
        A[n-1] = 0 # Backtracking choice: set bit to 0
        Binary(n - 1, A) # Recur for remaining bits
        A[n-1] = 1 # Backtracking choice: set bit to 1
        Binary(n - 1, A) # Recur for remaining bits
```

- **Recurrence**: $T(n) = 2T(n-1) + d$ for $n \ge 0$, and $T(n) = c$ for $n < 0$.

$$
T(n) =
\begin{cases}
c & \text{if } n < 0 \\
2T(n-1) + d, & \text{otherwise}
\end{cases}
$$

- **Complexity**: Solving this recurrence yields $T(n) = O(2^n)$, which is optimal.

---

### 4. Generate all the strings of length $n$ drawn from $0 \dots k-1$

To generate all $k$-ary strings of length $n$, we generalize the binary backtracking process. Instead of just two choices ($0$ and $1$), we iterate through all possible digits from $0$ to $k-1$, assigning each to $A[n-1]$ and recursively generating the remaining prefix.

```python
def k_string(n, k, A=None):
    if A is None:
        A = [0] * n # Assume array A is initialized
    if n < 1:
        print("".join(map(str, A))) # Print the completed k-ary string
    else:
        for j in range(k):
            A[n-1] = j # Set current position to digit j
            k_string(n - 1, k, A) # Recur for remaining digits
```

- **Recurrence**: $T(n) = k T(n-1) + d$ for $n \ge 0$, and $T(n) = c$ for $n < 0$.

$$
T(n) =
\begin{cases}
c & \text{if } n < 0 \\
kT(n-1) + d, & \text{otherwise}
\end{cases}
$$

- **Complexity**: Solving this recurrence yields $T(n) = O(k^n)$.

---

### 5. Finding the length of connected cells of $1s$ (regions) in an matrix of $0s$ and

$1s$: Given a matrix, each of which may be $1$ or $0$. The filled cells that are connected form a region. Two cells are said to be connected if they are adjacent to each other horizontally, vertically or diagonally. There may be several regions in the matrix. How do you find the largest region (in terms of number of cells) in the matrix?

To find the largest connected region of 1s, we iterate through each cell of the matrix. If a cell contains a 1 that has not been visited yet, we start a recursive depth-first search in all 8 possible directions. A 2D boolean array of visited cells prevents double counting. Each search returns the number of cells in its region, and we track the maximum. Visited cells are never unmarked, so every cell is processed once and the total time is $O(\text{rows} \times \text{columns})$.

```python
def getval(A, i, j, L, H):
    # Returns the value at A[i][j] or 0 if index is out of bounds
    if i < 0 or i >= L or j < 0 or j >= H:
        return 0
    return A[i][j]

def findMaxBlock(A, r, c, L, H, cntarr):
    # Returns the number of cells in the region that contains (r, c)
    cntarr[r][c] = True # Mark current cell as visited
    size = 1

    # Search in all eight directions
    direction = [
        [-1, 0], [-1, -1], [0, -1], [1, -1],
        [1, 0], [1, 1], [0, 1], [-1, 1]
    ]
    for i in range(8):
        newi = r + direction[i][0]
        newj = c + direction[i][1]
        val = getval(A, newi, newj, L, H)
        if val > 0 and not cntarr[newi][newj]:
            size += findMaxBlock(A, newi, newj, L, H, cntarr)
    return size

def getMaxOnes(A, rmax, colmax):
    # Finds the maximum region of connected 1s in the matrix
    maxsize = 0
    # Create 2D array of visited flags
    cntarr = [[False] * colmax for _ in range(rmax)]

    for i in range(rmax):
        for j in range(colmax):
            if A[i][j] == 1 and not cntarr[i][j]:
                maxsize = max(maxsize, findMaxBlock(A, i, j, rmax, colmax, cntarr))
    return maxsize
```

---

### 6. Solve the recurrence $T(n) = 2T(n-1) + 2^n$

At each level of the recurrence tree, the number of problems is double from the previous level, while the amount of work being done in each problem is half from the previous level. Formally, the $i^{th}$ level has $2^i$ subproblems, each requiring $2^{n-i}$ work. Thus, the $i^{th}$ level requires exactly $2^n$ work. The depth of this tree is $n$, because at the $i^{th}$ level, the originating call is $T(n-i)$. Summing the work over all $n$ levels yields a total time complexity of $O(n 2^n)$.

```python
def recurrence_6(n):
    # Recursive model representing T(n) = 2T(n-1) + 2^n
    if n == 0:
        return 1
    return 2 * recurrence_6(n - 1) + 2**n
```

---

[[chapter-1-introduction.md|← Previous]] - [[chapter-3-linked-lists|Next →]]
