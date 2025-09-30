# Big O Cheat Sheet

## Big O Notations

| Notation        | Name        | Description                                                                                 |
| --------------- | ----------- | ------------------------------------------------------------------------------------------- |
| **O(1)**        | Constant    | No loops                                                                                    |
| **O(log N)**    | Logarithmic | Usually searching algorithms have log n if they are sorted (Binary Search)                  |
| **O(n)**        | Linear      | For loops, while loops through n items                                                      |
| **O(n log(n))** | Log Linear  | Usually sorting operations                                                                  |
| **O(n²)**       | Quadratic   | Every element in a collection needs to be compared to every other element. Two nested loops |
| **O(2ⁿ)**       | Exponential | Recursive algorithms that solve a problem of size N                                         |
| **O(n!)**       | Factorial   | You are adding a loop for every element                                                     |

### Important Notes

- Iterating through half a collection is still **O(n)**
- Two separate collections: **O(a × b)**

## What Can Cause Time Complexity in a Function?

- **Operations**: `+`, `-`, `*`, `/`
- **Comparisons**: `<`, `>`, `==`
- **Looping**: `for`, `while`
- **Outside Function calls**: `function()`

## Rule Book for Big O Analysis

### Rule 1: Always Worst Case

Consider the worst-case scenario for your algorithm.

### Rule 2: Remove Constants

Drop constant factors when expressing Big O notation.

### Rule 3: Different Inputs Should Have Different Variables

- **O(a + b)**: Steps in order
- **O(a × b)**: Nested steps (A and B arrays nested)
- Use `+` for steps in order
- Use `×` for nested steps

### Rule 4: Drop Non-Dominant Terms

Focus on the term that grows the fastest.

## What Causes Space Complexity?

- **Variables**
- **Data Structures**
- **Function Calls**
- **Allocation**
