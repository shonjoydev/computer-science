# Chapter 1: Introduction

## Contents <!-- omit from toc -->

- [1.1 Variables](#11-variables)
- [1.2 Data Types](#12-data-types)
- [1.3 Data Structures](#13-data-structures)
- [1.4 Abstract Data Types (ADTs)](#14-abstract-data-types-adts)
- [1.5 What is an Algorithm?](#15-what-is-an-algorithm)
- [1.6 Why the Analysis of Algorithms?](#16-why-the-analysis-of-algorithms)
- [1.7 Goal of the Analysis of Algorithms](#17-goal-of-the-analysis-of-algorithms)
- [1.8 What is Running Time Analysis?](#18-what-is-running-time-analysis)
- [1.9 How to Compare Algorithms](#19-how-to-compare-algorithms)
- [1.10 What is Rate of Growth?](#110-what-is-rate-of-growth)
- [1.11 Commonly Used Rates of Growth](#111-commonly-used-rates-of-growth)
- [1.12 Types of Analysis](#112-types-of-analysis)
- [1.13 Asymptotic Notation](#113-asymptotic-notation)
- [1.14 Big-O Notation](#114-big-o-notation)
- [1.15 Omega-Ω Notation](#115-omega-ω-notation)
- [1.16 Theta-Θ Notation](#116-theta-θ-notation)
- [1.17 Important Notes](#117-important-notes)
- [1.18 Why is it called Asymptotic Analysis?](#118-why-is-it-called-asymptotic-analysis)
- [1.19 Guidelines for Asymptotic Analysis](#119-guidelines-for-asymptotic-analysis)
- [1.20 Simplifying Properties of Asymptotic Notations](#120-simplifying-properties-of-asymptotic-notations)
- [1.21 Commonly Used Logarithms and Summations](#121-commonly-used-logarithms-and-summations)
- [1.22 Master Theorem for Divide and Conquer Recurrences](#122-master-theorem-for-divide-and-conquer-recurrences)
- [1.23 Divide and Conquer Master Theorem: Problems \& Solutions](#123-divide-and-conquer-master-theorem-problems--solutions)
- [1.24 Master Theorem for Subtract and Conquer Recurrences](#124-master-theorem-for-subtract-and-conquer-recurrences)
- [1.25 Variant of Subtraction and Conquer Master Theorem](#125-variant-of-subtraction-and-conquer-master-theorem)
- [1.26 Method of Guessing and Confirming](#126-method-of-guessing-and-confirming)
- [1.27 Amortized Analysis](#127-amortized-analysis)
- [1.28 Algorithms Analysis: Problems \& Solutions](#128-algorithms-analysis-problems--solutions)

---

## 1.1 Variables

Before going to the definition of variables, let us relate them to old mathematical equations. All of us have solved many mathematical equations since childhood. As an example, consider the equation below:

$$x^2 + 2y - 2 = 1$$

We do not have to worry about the use of this equation. The important thing that we need to understand is that the equation has names ($x$ and $y$), which hold values (data). That means the names ($x$ and $y$) are placeholders for representing data. Similarly, in computer science programming we need something for holding data, and **variables** is the way to do that.

---

## 1.2 Data Types

In the above-mentioned equation, the variables $x$ and $y$ can take any values such as integral numbers ($10$, $20$), real numbers ($0.23$, $5.5$), or just $0$ and $1$. To solve the equation, we need to relate them to the kind of values they can take, and **data type** is the name used in computer science programming for this purpose. A data type in a programming language is a set of data with predefined values. Examples of data types are: integer, floating point, unit number, character, string, etc.

Computer memory is filled with zeros and ones. If we have a problem and we want to code it, it's very difficult to provide the solution in terms of zeros and ones. To help users, programming languages and compilers provide us with data types. For example, integer takes 2 bytes (actual value depends on compiler), float takes 4 bytes, etc. This says that in memory we are combining 2 bytes (16 bits) and calling it an integer. Similarly, combining 4 bytes (32 bits) and calling it a float. A data type reduces the coding effort. At the top level, there are two types of data types:

1. System-defined data types (also called Primitive data types)
2. User-defined data types

### System-defined Data Types

Data types that are defined by the system are called primitive data types. The primitive data types provided by many programming languages are: `int`, `float`, `char`, `double`, `bool`, etc. The number of bits allocated for each primitive data type depends on the programming languages, the compiler, and the operating system. For the same primitive data type, different languages may use different sizes. Depending on the size of the data types, the total available values (domain) will also change.

For example, `int` may take 2 bytes or 4 bytes. If it takes 2 bytes (16 bits), then the total possible values are $-32,768$ to $+32,767$ ($-2^{15}$ to $2^{15}-1$). If it takes 4 bytes (32 bits), then the possible values are between $-2,147,483,648$ and $+2,147,483,647$ ($-2^{31}$ to $2^{31}-1$). The same is the case with other data types.

### User-defined Data Types

If the system-defined data types are not enough, then most programming languages allow the users to define their own data types, called **user-defined data types**. Good examples of user-defined data types are structures in C/C++ and classes in Java.

---

## 1.3 Data Structures

Based on the discussion above, once we have data in variables, we need some mechanism for manipulating that data to solve problems. **Data structure** is a particular way of storing and organizing data in a computer so that it can be used efficiently. A data structure is a special format for organizing and storing data. General data structure types include arrays, files, linked lists, stacks, queues, trees, graphs, and so on.

Depending on the organization of the elements, data structures are classified into two types:

1. **Linear data structures**: Elements are accessed in a sequential order but it is not compulsory to store all elements sequentially. Examples: Linked Lists, Stacks, and Queues.
2. **Non-linear data structures**: Elements of this data structure are stored/accessed in a non-linear order. Examples: Trees and graphs.

---

## 1.4 Abstract Data Types (ADTs)

Before defining abstract data types, let us consider the different view of system-defined data types. We all know that, by default, all primitive data types (`int`, `float`, etc.) support basic operations such as addition and subtraction. The system provides the implementations for the primitive data types. For user-defined data types we also need to define operations. The implementation for these operations can be done when we want to actually use them. That means, in general, user-defined data types are defined along with their operations.

To simplify the process of solving problems, we combine the data structures with their operations and we call this **Abstract Data Types (ADTs)**. An ADT consists of two parts:

1. Declaration of data
2. Declaration of operations

Commonly used ADTs include: Linked Lists, Stacks, Queues, Priority Queues, Binary Trees, Dictionaries, Disjoint Sets (Union and Find), Hash Tables, Graphs, and many others. For example, stack uses LIFO (Last-In-First-Out) mechanism while storing the data in data structures. The last element inserted into the stack is the first element that gets deleted. Common operations of it are: creating the stack, pushing an element onto the stack, popping an element from the stack, finding the current top of the stack, finding the number of elements in the stack, etc.

While defining the ADTs do not worry about the implementation details. They come into the picture only when we want to use them. Different kinds of ADTs are suited to different kinds of applications, and some are highly specialized to specific tasks.

---

## 1.5 What is an Algorithm?

### Example: Making Coffee

Consider the problem of preparing a cup of coffee. We follow these steps:

1. Get the kettle.
2. Get the coffee powder.
   - Do we have coffee powder?
     - If yes, put a spoonful in the cup.
     - If no, do we want to buy coffee powder?
       - If yes, go out and buy it.
       - If no, terminate.
3. Boil the water.
4. Pour the hot water into the cup, add sugar/milk, and stir.
5. Serve.

For a given problem (making coffee), we are providing a **step-by-step procedure** for solving it.

### Definition

> An **algorithm** is a step-by-step, unambiguous set of instructions to solve a given problem.

### Criteria for Judging Algorithms

In the traditional study of algorithms, there are two main criteria:

| Criterion       | Question it answers                                                            |
| --------------- | ------------------------------------------------------------------------------ |
| **Correctness** | Does the algorithm give a solution to the problem in a finite number of steps? |
| **Efficiency**  | How many resources (memory and time) does it take to execute?                  |

**Note:** We do not have to prove each step of the algorithm

## 1.6 Why the Analysis of Algorithms?

To go from city "A" to city "B", there can be many ways of accomplishing this: by flight, by bus, by train, and also by bicycle. Depending on the availability and convenience, we choose the one that suits us. Similarly, in computer science, multiple algorithms are available for solving the same problem (for example, a sorting problem has many algorithms, like insertion sort, selection sort, quick sort, and many more). **Algorithm analysis** helps us to determine which algorithm is most efficient in terms of time and space consumed.

---

## 1.7 Goal of the Analysis of Algorithms

The goal of the analysis of algorithms is to compare algorithms (or solutions) mainly in terms of running time but also in terms of other factors (e.g., memory, developer effort, etc.).

---

## 1.8 What is Running Time Analysis?

It is the process of determining how processing time increases as the size of the problem (input size) increases. Input size is the number of elements in the input, and depending on the problem type, the input may be of different types. The following are the common types of inputs:

- Size of an array
- Polynomial degree
- Number of elements in a matrix
- Number of bits in the binary representation of the input
- Vertices and edges in a graph

---

## 1.9 How to Compare Algorithms

To compare algorithms, let us define a few objective measures:

- **Execution times?** Not a good measure as execution times are specific to a particular computer.
- **Number of statements executed?** Not a good measure, since the number of statements varies with the programming language as well as the style of the individual programmer.
- **Ideal solution?** Let us assume that we express the running time of a given algorithm as a function of the input size $n$ (i.e., $f(n)$) and compare these different functions corresponding to running times. This kind of comparison is independent of machine time, programming style, etc.

---

## 1.10 What is Rate of Growth?

The rate at which the running time increases as a function of input is called the **rate of growth**. Let us assume that you go to a shop to buy a car and a bicycle. If your friend sees you there and asks what you are buying, then in general you say buying a car. This is because the cost of the car is high compared to the cost of the bicycle (approximating the cost of the bicycle to the cost of the car).

$$
\text{Total Cost} = \text{cost\_of\_car} + \text{cost\_of\_bicycle}
\approx \text{cost\_of\_car}
$$

For the above-mentioned example, we can represent the cost of the car and the cost of the bicycle in terms of function, and for a given function ignore the low order terms that are relatively insignificant (for large values of input size, $n$). As an example, in the case below, $n^4$, $2n^2$, $100n$ and $500$ are the individual costs of some function and approximate to $n^4$ since $n^4$ is the highest rate of growth.

$$n^4 + 2n^2 + 100n + 500 \approx n^4$$

---

## 1.11 Commonly Used Rates of Growth

Below is the list of growth rates you will come across in the following chapters, ordered from lowest rate of growth (most efficient) to highest [37]:

| Time Complexity | Name               | Example                                               |
| :-------------- | :----------------- | :---------------------------------------------------- |
| $1$             | Constant           | Adding an element to the front of a linked list       |
| $\log n$        | Logarithmic        | Finding an element in a sorted array                  |
| $n$             | Linear             | Finding an element in an unsorted array               |
| $n \log n$      | Linear Logarithmic | Sorting $n$ items by 'divide-and-conquer' - Mergesort |
| $n^2$           | Quadratic          | Shortest path between two nodes in a graph            |
| $n^3$           | Cubic              | Matrix Multiplication                                 |
| $2^n$           | Exponential        | The Towers of Hanoi problem                           |

---

## 1.12 Types of Analysis

To analyze a given algorithm, we need to know with which inputs the algorithm takes less time (performing well) and with which inputs the algorithm takes a long time. We represent the algorithm with multiple expressions: one for the case where it takes less time (best case) and another for the case where it takes more time (worst case).

There are three types of analysis:

- **Worst case**: Defines the input for which the algorithm takes the longest time (slowest time to complete). The input is the one for which the algorithm runs the slowest.
- **Best case**: Defines the input for which the algorithm takes the least time (fastest time to complete). The input is the one for which the algorithm runs the fastest.
- **Average case**: Provides a prediction about the running time of the algorithm. We run the algorithm many times, using many different inputs that come from some distribution that generates these inputs, compute the total running time, and divide by the number of trials. It assumes that the input is random.

$$
Lower\ Bound \le Average\ Time \le Upper\ Bound
$$

---

## 1.13 Asymptotic Notation

Having the expressions for the best, average, and worst cases, we need to identify their upper and lower bounds. To represent these upper and lower bounds, we use asymptotic notations, which represent a curve approximating the algorithm's actual performance at higher values of $n$.

---

## 1.14 Big-O Notation

**[Upper Bounding Function]**

This notation gives the tight upper bound of the given function. Generally, it is represented as $f(n) = O(g(n))$. That means, at larger values of $n$, the upper bound of $f(n)$ is $g(n)$.

$$
O(g(n)) = \{ f(n) : \text{there exist positive constants } c
\text{ and } n_0 \text{ such that } 0 \le f(n) \le c \cdot g(n)
\text{ for all } n > n_0 \}
$$

Our objective is to give the smallest rate of growth $g(n)$ which is greater than or equal to the given algorithm's rate of growth $f(n)$. We discard lower values of $n$ (below the threshold $n_0$).

- $O(1)$: $100, 1000, 200, 1, 20$
- $O(n)$: $3n+100, 100n, 2n-1$
- $O(n \log n)$: $5n \log n, 3n-100, 100n$
- $O(n^2)$: $n^2, 5n-10, n^2-2n+1$

## 1.15 Omega-Ω Notation

**[Lower Bounding Function]**

This notation gives the tighter lower bound of the given algorithm and we represent it as $f(n) = \Omega(g(n))$. That means, at larger values of $n$, the tighter lower bound of $f(n)$ is $g(n)$.

$$
\Omega(g(n)) = \{ f(n) : \text{there exist positive constants } c
\text{ and } n_0 \text{ such that } 0 \le c \cdot g(n) \le f(n)
\text{ for all } n \ge n_0 \}
$$

Our objective is to give the largest rate of growth $g(n)$ which is less than or equal to the given algorithm's rate of growth $f(n)$.

## 1.16 Theta-Θ Notation

**[Order Function]**

This notation decides whether the upper and lower bounds of a given function (algorithm) are the same. The average running time of an algorithm is always between the lower bound and the upper bound. If the upper bound ($O$) and lower bound ($\Omega$) give the same rate of growth, then the $\Theta$ notation will also have the same rate of growth.

$$
\Theta(g(n)) = \{ f(n) : \text{there exist positive constants } c_1, c_2
\text{ and } n_0 \text{ such that } 0 \le c_1 \cdot g(n) \le f(n) \le c_2 \cdot g(n)
\text{ for all } n \ge n_0 \}
$$

$\Theta(g(n))$ is the set of functions with the same order of growth as $g(n)$.

---

## 1.17 Important Notes

For analysis (best case, worst case, and average), we try to give the upper bound ($O$), lower bound ($\Omega$), and average running time ($\Theta$). Getting all three may not always be possible. In practice, we generally focus on the upper bound ($O$) because knowing the lower bound ($\Omega$) of an algorithm is of no practical importance. We use the $\Theta$ notation if the upper bound ($O$) and lower bound ($\Omega$) are the same.

---

## 1.18 Why is it called Asymptotic Analysis?

In every case, for a given function $f(n)$, we are trying to find another function $g(n)$ which approximates $f(n)$ at higher values of $n$. In mathematics, we call such a curve an **asymptotic curve**. For this reason, we call algorithm analysis **asymptotic analysis**.

---

## 1.19 Guidelines for Asymptotic Analysis

There are some general rules to help us determine the running time of an algorithm:

### 1. Loops

The running time of a loop is, at most, the running time of the statements inside the loop (including tests) multiplied by the number of iterations.

```python
def loop_example(n):
    m = 0
    for i in range(1, n + 1): # Executes n times
        m = m + 2 # Constant time, c
    return m
```

$\text{Total time = a constant } c × n = c n = O(n)$.

### 2. Nested Loops

Analyze from the inside out. The total running time is the product of the sizes of all the loops.

```python
def nested_loop_example(n):
    k = 0

    # outer loop executed n times
    for i in range(1, n + 1):
        # inner loop executes n times
        for j in range(1, n + 1):
            k = k + 1 # Constant time, c
    return k
```

$\text{Total time = a constant } c \times n \times n = cn^2 = O(n^2)$

### 3. Consecutive Statements

Add the time complexities of each statement.

```python
def consecutive_statements_example(n):
    x = 0
    x = x + 1 # Constant time

    m = 0
    for i in range(1, n + 1):
        m = m + 2 # O(n)

    k = 0
    for i in range(1, n + 1):
        for j in range(1, n + 1):
            k = k + 1 # O(n^2)
    return x, m, k
```

$\text{Total time = } c_0 + c_1n + c_2n^2 = O(n^2)$

### 4. If-then-else Statements

Worst-case running time: the test, plus either the then part or the else part (whichever is larger).

```python
def compare_lists(list1, other_list):
    if len(list1) == 0:                   # Constant: c
        return False                      # Constant: c

    else:
        for n in range(len(list1)):       # Constant + Constant: c + c, repeated n times
            if list1[n] == other_list[n]: # Constant + Constant: c + c
                return False              # Constant: c

    return True                           # Constant: c
```

$$
\text{Total time} = c_0 + c_1 + (c_2 + c_3 + c_4) \times n + c_5 = O(n)
$$

$$
\text{Final complexity}: \boxed{O(n)}
$$

### 5. Logarithmic Complexity

An algorithm is $O(\log n)$ if it takes a constant time to cut the problem size by a fraction (usually by $1/2$).

```python
def logarithmic_example(n):
    i = 1                 # c₀
    count = 0             # c₁

    while i <= n:         # c₂, repeated log₂(n) + 1 times
        i = i * 2         # c₃, repeated log₂(n) times
        count += 1        # c₄, repeated log₂(n) times

    return count          # c₅
```

$$
\begin{aligned}

\text{Total time}
&= c_0 + c_1 + c_2(\log_2 n + 1) + (c_3 + c_4)\log_2 n + c_5 \\
&= O(\log n)
\end{aligned}
$$

```python
def divide_by_two(n):
    i = n              # c₀

    while i >= 1:      # c₁, repeated log₂(n) + 1 times
        i = i / 2      # c₂, repeated log₂(n) + 1 times

    return i           # c₃
```

$$
\text{Total time}
= c_0 + c_1(\log_2 n + 1) + c_2(\log_2 n + 1) + c_3
= O(\log n)
$$

---

## 1.20 Simplifying Properties of Asymptotic Notations

- **Transitivity**: $f(n) = \Theta(g(n))$ and $g(n) = \Theta(h(n)) \Rightarrow f(n) = \Theta(h(n))$. Valid for $O$ and $\Omega$ as well.
- **Reflexivity**: $f(n) = \Theta(f(n))$. Valid for $O$ and $\Omega$.
- **Symmetry**: $f(n) = \Theta(g(n))$ if and only if $g(n) = \Theta(f(n))$.
- **Transpose symmetry**: $f(n) = O(g(n))$ if and only if $g(n) = \Omega(f(n))$.
- If $f(n)$ is in $O(k \cdot g(n))$ for any constant $k > 0$, then $f(n)$ is in $O(g(n))$.
- If $f_1(n)$ is in $O(g_1(n))$ and $f_2(n)$ is in $O(g_2(n))$, then $(f_1+f_2)(n)$ is in $O(\max(g_1(n), g_2(n)))$.
- If $f_1(n)$ is in $O(g_1(n))$ and $f_2(n)$ is in $O(g_2(n))$, then $f_1(n)f_2(n)$ is in $O(g_1(n)g_2(n))$.

---

## 1.21 Commonly Used Logarithms and Summations

### Logarithms

- $\log x^y = y \log x$
- $\log xy = \log x + \log y$
- $\log \frac{x}{y} = \log x - \log y$
- $\log^kn = (\log n)^k$
- $\log_b x = \frac{\log_a x}{\log_a b}$
- $a^{\log_b x} = x^{\log_b a}$

### Arithmetic Series

$$\sum_{k=1}^{n} k = 1 + 2 + \dots + n = \frac{n(n+1)}{2}$$

### Geometric Series

$$
\sum_{k=0}^{n} x^k = 1 + x + x^2 + \dots + x^n = \frac{x^{n+1}-1}{x-1} \quad (x \not ={1})
$$

### Harmonic Series

$$\sum_{k=1}^{n} \frac{1}{k} = 1 + \frac{1}{2} + \dots + \frac{1}{n} \approx \log n$$

### Other important formulae

$$\sum_{k=1}^{n} log \ k \approx n\log n$$

$$
\sum_{k=1}^{n} k^p = 1^p + 2^p  + \dots + x^p = \frac{1}{p+1} n^{p+1}
$$

---

## 1.22 Master Theorem for Divide and Conquer Recurrences

All divide and conquer algorithms divide the problem into sub-problems, each of which is part of the original problem, and then perform some additional work to compute the final answer.

If the recurrence is of the form $T(n) = aT(n/b) + \Theta(n^k \log^p n)$, where $a \ge 1, b > 1, k \ge 0$, and $p$ is a real number, then:

1. **If $a > b^k$**, then $T(n) = \Theta(n^{\log_b a})$.
2. **If $a = b^k$**:
   - a. If $p > -1$, then $T(n) = \Theta(n^{\log_b a} \log^{p+1} n)$
   - b. If $p = -1$, then $T(n) = \Theta(n^{\log_b a} \log \log n)$
   - c. If $p < -1$, then $T(n) = \Theta(n^{\log_b a})$
3. **If $a < b^k$**:
   - a. If $p \ge 0$, then $T(n) = \Theta(n^k \log^p n)$
   - b. If $p < 0$, then $T(n) = O(n^k)$

---

## 1.23 Divide and Conquer Master Theorem: Problems & Solutions

### 1. Solve $T(n) = 3T(n/2) + n^2$

- Solution: $a=3, b=2, k=2, p=0$. Since $3 < 2^2$ (Case 3.a applies with $p \ge 0$), we get $T(n) = \Theta(n^2)$.

### 2. Solve $T(n) = 4T(n/2) + n^2$

- Solution: $a=4, b=2, k=2, p=0$. Since $4 = 2^2$ (Case 2.a applies with $p = 0 > -1$), we get $T(n) = \Theta(n^2 \log n)$.

### 3. Solve $T(n) = T(n/2) + n^2$

- Solution: $a=1, b=2, k=2, p=0$. Since $1 < 2^2$ (Case 3.a applies), we get $T(n) = \Theta(n^2)$.

### 4. Solve $T(n) = 2^n T(n/2) + n^n$

- Solution: Master Theorem does not apply because $a=2^n$ is not a constant.

### 5. Solve $T(n) = 16T(n/4) + n$

- Solution: $a=16, b=4, k=1, p=0$. Since $16 > 4^1$ (Case 1 applies), we get $T(n) = \Theta(n^{\log_4 16}) = \Theta(n^2)$.

### 6. Solve $T(n) = 2T(n/2) + n \log n$

- Solution: $a=2, b=2, k=1, p=1$. Since $2 = 2^1$ (Case 2.a applies with $p = 1 > -1$), we get $T(n) = \Theta(n \log^2 n)$.

### 7. Solve $T(n) = 2T(n/2) + n/\log n$

- Solution: $a=2, b=2, k=1, p=-1$. Since $2 = 2^1$ (Case 2.b applies with $p = -1$), we get $T(n) = \Theta(n \log \log n)$.

### 8. Solve $T(n) = 2T(n/4) + n^{0.51}$

- Solution: $a=2, b=4, k=0.51, p=0$. Since $2 < 4^{0.51}$ (Case 3.b applies), we get $T(n) = \Theta(n^{0.51})$.

### 9. Solve $T(n) = 0.5T(n/2) + 1/n$

- Solution: Master Theorem does not apply because $a = 0.5 < 1$.

### 10. Solve $T(n) = 6T(n/3) + n^2 \log n$

- Solution: $a=6, b=3, k=2, p=1$. Since $6 < 3^2$ (Case 3.a applies), we get $T(n) = \Theta(n^2 \log n)$.

---

## 1.24 Master Theorem for Subtract and Conquer Recurrences

Let $T(n)$ be a function defined on positive $n$ having the property:

$$
T(n) =
\begin{cases}
c, & \text{if } n \le 1 \\
aT(n-b) + f(n), & \text{if } n > 1
\end{cases}
$$

If $f(n)$ is in $O(n^k)$, then:

$$
T(n) =
\begin{cases}
O(n^k), & \text{if } a < 1 \\
O(n^{k+1}), & \text{if } a = 1 \\
O(n^k a^{n/b}), & \text{if } a > 1
\end{cases}
$$

---

## 1.25 Variant of Subtraction and Conquer Master Theorem

The solution to the equation $T(n) = T(\alpha n) + T((1-\alpha)n) + \beta n$, where $0 < \alpha < 1$ and $\beta > 0$ are constants, is $O(n \log n)$.

---

## 1.26 Method of Guessing and Confirming

For recurrences that do not match the Master Theorem format, we guess the answer and then prove it correct by induction. If the guess is incorrect, the mathematical failure of the proof helps us refine our guess.

For example, consider the recurrence:
$$T(n) = \sqrt{n}T(\sqrt{n}) + n$$

By guessing $T(n) = \Theta(n \log \log n)$, we can prove the tight upper and lower bounds using induction.

---

## 1.27 Amortized Analysis

Amortized analysis refers to determining the time-averaged running time for a sequence of operations. It is different from average-case analysis because it does not make any assumption about the distribution of the data. Amortized analysis is a worst-case analysis of a sequence of operations, demonstrating that while individual operations may be expensive, their average cost over a long sequence is low.

---

## 1.28 Algorithms Analysis: Problems & Solutions

### 21. Complexity of recurrence $T(n) = 3T(n-1)$ for $n > 0$, and $T(0) = 1$

$$
T(n) =
\begin{cases}
1 & \text{otherwise} \\
3T(n-1), & \text{if } n > 0
\end{cases}
$$

- Solution: Using substitution:

  $$
  \begin{aligned}
  T(n) &= 3T(n-1) \\
  T(n) &= 3(3T(n-2)) = 3^2T(n-2) \\
  T(n) &= 3^2(3T(n-3)) \\
       &\vdots \\
  T(n) &= 3^nT(n-n) \\
       &= 3^nT(0) \\
       &= 3^n\times1 \\
       &= 3^n
  \end{aligned}
  $$

- Shortcut:
  $$T(n) = 3T(n-1) = 3^2 T(n-2) = \dots = 3^n T(0) = 3^n$$
  The time complexity is $O(3^n)$.

### 22. Complexity of recurrence $T(n) = 2T(n-1) - 1$ for $n > 0$, and $T(0) = 1$

$$
T(n) =
\begin{cases}
1 & \text{otherwise} \\
2T(n-1)-1, & \text{if } n > 0
\end{cases}
$$

- Solution: Using substitution:

  $$
  \begin{aligned}
    T(n) &= 2T(n-1)-1 \\
    T(n) &= 2(2T(n-2)-1)-1 = 2^2T(n-2) - 2 - 1 \\
    T(n) &= 2^2(2T(n-3)-2-1)-1 = 2^3T(n-4)-2^2-2^1-2^0 \\
    T(n) &= 2^nT(n-n)-2^{n-1}-2^{n-2}-2^{n-3}\dots 2^2 - 2^1 - 2^0 \\
    T(n) &= 2^n - 2^{n-1} - 2^{n-2} - 2^{n-3} \dots 2^2 - 2^1 - 2^0 \\
    T(n) &= 2^n-(2^n-1)[note: 2^{n-1}+2^{n-2}+\dots+2^0 = 2^n] \\
    T(n) &= 1
  \end{aligned}
  $$

- Shortcut:
  $$T(n) = 2^n T(0) - (2^{n-1} + 2^{n-2} + \dots + 2^0) = 2^n - (2^n - 1) = 1$$
  The time complexity is $O(1)$.

### 23. What is the running time of the following function?

```python
def Function_23(n):
    i = 1
    s = 1
    while s <= n: # s is increasing not at rate 1 but i
        i += 1
        s = s + i
        print("*", end="")
```

- Explanation: We can define the $\text{s}$ terms according to the relation $s_i = s_{i–1} + i$. The value oft’ increases by $1$ for each iteration. The value contained in $s$ at the $i^{th}$ iteration is the sum of the first ‘(‘positive integers. If $k$ is the total number of iterations taken by the program, then the while loop terminates if:

$$1+2+\dots+k=\frac{k(k+1)}{2}>n \implies k = O(\sqrt{n})$$

- Explanation: The value of $s$ increases as the sum of consecutive integers: $s_k = \frac{k(k+1)}{2}$. The loop terminates when $\frac{k(k+1)}{2} > n$, giving $k = O(\sqrt{n})$.

### 24. Find the complexity of the function given below

```python
def function_24(n):
    count = 0
    i = 1
    while i * i <= n:
        count += 1
        i += 1
```

- Explanation: The loop terminates when $i^2 > n$, which means $i > \sqrt{n}$. Hence, the running time is $O(\sqrt{n})$.

### 25. Find the complexity of the program given below

```python
def function_25(n):
    count = 0
    # Outer loop executes n/2 times
    for i in range(n // 2, n + 1):
        # Middle loop executes n/2 times
        j = 1
        while j + n // 2 <= n:
            # Inner loop executes log(n) times
            k = 1
            while k <= n:
                count += 1
                k = k * 2
            j = j + 1
    return count
```

- Explanation: The outer loop runs $n/2$ times, the middle loop runs $n/2$ times, and the innermost loop runs $\log n$ times. The total complexity is $O(n^2 \log n)$.

### 26. Find the complexity of the program given below

```python
def function_26(n):
    count = 0
    # outer loop execute n/2 time
    for i in range(n // 2, n + 1):
        j = 1
        # middle loop executes log n times
        while j <= n:
            k = 1
            # inner loop execute log n times
            while k <= n:
                count += 1
                k = k * 2
            j = 2 * j
    return count
```

- Explanation: The outer loop executes $n/2$ times. The middle loop is logarithmic and runs $\log n$ times, as does the inner loop. The overall time complexity is $O(n \log^2 n)$.

### 27. Find the complexity of the program below

```python
def function_27(n):
    # constant time
    if n == 1:
        return

    # outer loop execute n times
    for i in range(1, n + 1):
        # inner loop executes only time due to break statement
        for j in range(1, n + 1):
            print("*", end="")
            break # Breaks inner loop immediately
```

- Explanation: Although the inner loop is bounded by $n$, due to the `break` statement, it executes only once per outer iteration. Thus, the complexity is $O(n)$.

### 28. Express running time of recursive function as a recurrence

```python
def function_28(n):
    # constant time
    if n <= 1:
        return
    # outer loop execute n times
    for i in range(1, n + 1):
        # inner loop executes n times
        for j in range(1, n + 1):
            # constant time
            print("*", end="")
    function_28(n - 3)
```

- Explanation: The function executes $n^2$ print operations in the nested loops, and then calls itself recursively with size $n-3$. This yields the recurrence $T(n) = T(n-3) + c n^2$, which solves to $T(n) = \Theta(n^3)$ by Subtract & Conquer.

### 32. Prove that the running time of the code below is Ω(log n)

```python
def Read_32(n):
    k = 1
    while k < n:
        k = 3 * k
```

- Explanation: The value of $k$ is multiplied by 3 at each iteration, meaning after $i$ iterations, $k = 3^i$. The loop terminates when $3^i \ge n$, indicating $i \ge \log_3 n = \Omega(\log n)$.

### 34. Find running time of recursive Fibonacci

```python
def fib(n):
    if n == 0:
        return 0
    elif n == 1:
        return 1
    else:
        return fib(n - 1) + fib(n - 2)
```

- Explanation: The recurrence relation is $T(n) = T(n-1) + T(n-2) + c$. This generates a binary tree of calls of depth $n$, containing $O(2^n)$ leaves, leading to exponential complexity $O(2^n)$.

### 35. Find running time of the program below

```python
def function_35(n):
    # this loop executes n times
    for i in range(1, n + 1):
        j = 1
        # this loop executes j times with increase by the rate of i
        while j <= n:
            print("*", end="")
            j += i
```

- Explanation: The inner loop executes $\lceil n/i \rceil$ times for each value of $i$. The total running time is proportional to $n \sum_{i=1}^n \frac{1}{i}$, which is the harmonic series and evaluates to $O(n \log n)$.

### 37. Find running time of the following recursive function

```python
import math
def function_37(n):
    # constant time
    if n <= 1:
        return
    # this loop executes with recursive loop of n/3 value
    for i in range(1, 4):
        function_37(math.ceil(n / 3))
```

- Explanation: The recurrence relation is $T(n) = 3T(n/3) + \Theta(1)$. By the Master Theorem, $a=3, b=3, k=0, p=0$, so $T(n) = \Theta(n)$.

### 38. Find running time of the following recursive function

```python
def function_38(n):
    # constant time
    if n <= 1:
        return
    # this loop executes 3 times with recursive call of n-1 value
    for i in range(1, 4):
        function_38(n - 1)
```

- Explanation: The recurrence relation is $T(n) = 3T(n-1) + c$. Using the Subtract & Conquer Master Theorem with $a=3, b=1$, we find the complexity is $O(3^n)$.

### 39. Express running time of recursive function as a recurrence

```python
def function_39(n):
    # constant time
    if n <= 1:
        return
    # this loop executes n times with constant time loop
    for i in range(1, int(n)):
        print("*", end="")
    # recursive call with 0.8n
    function_39(int(0.8 * n))
```

- Explanation: The function performs $n$ constant-time print statements and calls itself recursively with size $0.8n$. This yields $T(n) = T(4/5 n) + O(n)$, which solves to $T(n) = O(n)$ by the Master Theorem.

### 43. Analyze running time of the following recursive function

```python
import math
def Function_43(n):
    if n <= 2:
        return 1
    else:
        return Function_43(math.floor(math.sqrt(n))) + 1
```

- Explanation: The recurrence relation is $T(n) = T(\sqrt{n}) + 1$. To solve, let $n = 2^m \Rightarrow m = \log n$. Then $S(m) = S(m/2) + 1$, which solves to $S(m) = O(\log m)$. Substituting back gives $T(n) = O(\log \log n)$.

### 44. Find complexity of the program below

```python
def function_44(n):
    # constant time
    if n < 2:
        return
    else:
        counter = 0
        # this loop executes 8 times with n value half in every call
        for i in range(1, 9):
            function_44(n // 2)
        # this loop executes n³ times with constant time loop
        for i in range(1, n**3 + 1):
            counter += 1
```

- Explanation: The recurrence relation is $T(n) = 8T(n/2) + \Theta(n^3)$. By the Master Theorem, $a=8, b=2, k=3, p=0$, since $8 = 2^3$ (Case 2.a), we get $T(n) = \Theta(n^3 \log n)$.

### 45. Find the complexity of the pseudocode below

```python
def function_45(n):
    temp = 1 # constant time
    # this loop executes log n times, since n is halved on every pass
    while n > 1:
        for i in range(1, n + 1):
            temp = temp + 1
        # halve n for the next pass (iterative, not a recursive call)
        n = n // 2
```

- Explanation: The recurrence for this work is $T(n) = T(n/2) + n$. By the Master Theorem, $a=1, b=2, k=1, p=0$, since $1 < 2^1$ (Case 3.a), we get $T(n) = O(n)$.

### 46. Find the complexity of the following program

```python
def function_46(n):
    # this loop executes n times
    for i in range(1, n + 1):
        j = 1
        # this loops executes log n times from our logarithms guideline
        while j <= n:
            print("*", end="")
            j *= 2
```

- Explanation: The outer loop runs $n$ times. The inner loop is logarithmic, running $\log n$ times. Thus, the complexity is $O(n \log n)$.

### 47. Find the complexity of the following program

```python
def function_47(n):
    # this loops executes n/3 times
    for i in range(1, n // 3 + 1):
        # this loop executes n/4 times
        for j in range(1, n + 1, 4):
            print("*", end="")
```

- Explanation: The outer loop runs $n/3$ times, and the inner loop runs $n/4$ times. The overall time complexity is $O(n^2)$.

### 48. Find the complexity of the following program

```python
def function_48(n):
    if n <= 1:
        return
    if n > 1:
        print("*", end="")
        function_48(n // 2)
        function_48(n // 2)
```

- Explanation: The recurrence relation is $T(n) = 2T(n/2) + 1$. By the Master Theorem, $a=2, b=2, k=0, p=0$, since $2 > 2^0$, we get $T(n) = \Theta(n)$.

### 49. Find the complexity of the following program

```python
def function_49(n):
    i = 1
    while i < n:
        j = n
        while j > 0:
            j = j // 2 # log n code
        i = 2 * i # log n times
```

- Explanation: The outer loop runs $\log n$ times because $i$ is doubled in each step. The inner loop runs $\log n$ times because $j$ is halved in each step. The overall time complexity is $O(\log^2 n)$.

### 53. Find the number of comparisons made in the loop below

```python
def loop_53(n):
    j = 1
    while j <= n:
        j = j * 2
```

- Explanation: The value of $j$ doubles at each step: $j_k = 2^k$. The loop body runs while $2^k \le n$, that is $\lfloor \log_2 n \rfloor + 1$ times, and the condition is checked one more time at the end to exit. Thus, the number of comparisons made is $\lfloor \log_2 n \rfloor + 2 = O(\log n)$.

### 54. Find the execution bounds of the loop in the prime checking code

```python
import math
def IsPrime(n):
    # Checks if n is prime by scanning up to sqrt(n)
    for i in range(2, int(math.sqrt(n)) + 1):
        if n % i == 0:
            print("Not Prime")
            return 0
    return 1
```

- Explanation: The loop runs a maximum of $\sqrt{n}$ times (when $n$ is prime) and a minimum of 1 time (when $n$ is even). Therefore, the loop execution complexity is $T(n) = O(\sqrt{n})$ and $T(n) = \Omega(1)$.

### 55. Find the complexity of the recursive GCD function

```python
def gcd(n, m):
    if n % m == 0:
        return m
    n = n % m
    return gcd(m, n)
```

- Explanation: The running time varies significantly based on input. For $m=2$ and $n=2^i$, the loop runs in $O(1)$ time, which contradicts simple static bounds.

### 57. Find the complexity of the program below

```python
def function_57(n):
    # executes n times
    for i in range(0, n):
        # executes n*n times
        for j in range(i, i * i):
            if j % i == 0:
                # executes j times = (n*n) times
                for k in range(0, j):
                    print(" * ", end="")
```

- Explanation: The outer loop runs $n$ times. The middle loop runs from $i$ to $i^2$, and the innermost loop runs $j$ times when $j$ is a multiple of $i$. This leads to a total time complexity of $O(n^5)$.

### 63. Find the complexity of the program below

```python
def function_63(n, j):
    sum_val = 0
    # executes n times
    for i in range(0, n):
        if i > j:
            # executes n times
            sum_val = sum_val + 1
        else:
            # executes n times
            for k in range(0, n):
                sum_val = sum_val - 1
    return sum_val
```

- Explanation: In the worst-case, $i \le j$ for all iterations, executing the inner loop $n$ times during each outer loop pass. The worst-case complexity is $O(n^2)$.

---

[[chapter-2-recursion-and-backtracking.md|Next →]]
