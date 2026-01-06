# Algorithms — Day 01 (Frequency Count Method)

## Topic  
**Analyzing Time Complexity Using the Frequency Count Method**

This session introduced the **Frequency Count Method**, a systematic way to analyze the time complexity of an algorithm by counting how many times each statement executes.

---

## Concept Overview

The Frequency Count Method evaluates an algorithm by:
- Counting the number of times each instruction runs
- Expressing the total execution cost as a **function of input size (n)**
- Converting that function into **time complexity**

This approach helps in understanding the performance of an algorithm **before actual execution**.

---

## Example Algorithm

**Algorithm:** `Sum(A, n)`  
Purpose: Calculate the sum of all elements in an array.

### Pseudocode
Sum(A, n)
{
    s = 0
    for i = 0 to n-1
        s = s + A[i]
        return s
}

---

## Frequency Count Analysis

| Statement | Frequency |
|-----------|-----------|
| `s = 0` | 1 |
| `i = 0` (initialization) | 1 |
| `i < n` (condition check) | n + 1 |
| `i++` (increment) | n |
| `s = s + A[i]` | n |
| `return s` | 1 |

---

## Total Cost Function

Adding all frequencies:

f(n) = 2n + 3

### Final Result  
The time complexity of the algorithm is:

**O(n)** — Linear Time

---

## Key Learnings

- The Frequency Count Method gives a **clear mathematical model** of execution cost.  
- It helps in understanding **why** an algorithm is O(n), O(n²), etc.  
- Constants do not matter in Big-O notation; **growth rate matters**.  
- This method is useful for:
  - Comparing algorithms
  - Predicting scalability
  - Improving performance

---

## Personal Understanding

> “Before measuring speed in seconds, measure work in steps.”

From now on, I will:
- First count the number of operations.  
- Then derive the complexity.  
- Finally, optimize the logic if needed.

---

## Learning Resource

Algorithms Playlist  
https://www.youtube.com/playlist?list=PLDN4rrl48XKpZkf03iYFl-O29szjTrs_O
