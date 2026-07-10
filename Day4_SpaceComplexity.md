#  Chapter 04: Space Complexity (Part 1)

# Table of Contents (Part 1)

1. What is Space Complexity?
2. Why Do We Need Space Complexity?
3. Memory in Computer
4. Types of Memory Used by an Algorithm
5. Real-Life Example
6. Space Complexity Notation
7. Basic Examples
8. Important Notes
9. Interview Questions
---

# 1  What is Space Complexity?

##  English
**Space Complexity** is the total amount of memory required by an algorithm to execute completely.
It includes all the memory used by the program during execution.

##  Hindi
**Space Complexity** ka matlab hai kisi algorithm ko execute hone ke liye kitni memory ki zarurat padti hai.
Ye program ke execution ke dauran use hone wali total memory ko represent karti hai.

#  Exam Definition
**Space Complexity** is the total memory required by an algorithm during its execution.

# 2 Why Do We Need Space Complexity?
Imagine your mobile has only **64 GB storage**.
If one application uses **40 GB RAM**, your phone will become slow or may even crash.
Similarly,
An algorithm that uses more memory is less efficient.
Therefore,
we always try to reduce memory usage.

#  Real-Life Example
Imagine you are going on a trip.
You have only **one small backpack**.
If you pack only necessary items,
* Easy to carry
--If you pack unnecessary things,
* Heavy bag
* Difficult to travel
Similarly,
Algorithms should use only the required memory.

# 3 Memory Used by an Algorithm
Whenever a program runs,
it uses memory for:
- Variables
- Arrays
- Objects
- Function Calls
- Recursion
- Temporary Variables

# Memory Representation
```
Program Memory
│
├── Variables
├── Arrays
├── Objects
├── Functions
└── Temporary Memory
```

#  Types of Memory
Space Complexity mainly consists of two parts.

```
Space Complexity
│
├── Input Space
└── Auxiliary Space
```

## A. Input Space

###  English
Input Space is the memory required to store the input data.

###  Hindi
Input Space woh memory hoti hai jo input data ko store karne ke liye use hoti hai.

### Example:

```java
int arr[] = new int[100];
```
Here,
the array itself is the input.

## B. Auxiliary Space

### English
Auxiliary Space is the extra memory used by the algorithm apart from the input.

### Hindi
Auxiliary Space algorithm ke dwara use ki gayi extra memory hoti hai.

### Example:

```java
int temp;
```
Here,
`temp` is extra memory.

#  Important Formula

```
Space Complexity
=
Input Space
+
Auxiliary Space
```

# 5 Basic Example

```java
int a = 10;
int b = 20;
int sum = a + b;
```

Variables used
```
a
b
sum
```
Only three variables are created.
Hence,
Space Complexity = **O(1)**
(Constant Space)

# 6 Another Example
```java
int arr[] = new int[n];
```

If `n` increases,
memory also increases.
Therefore,
Space Complexity = **O(n)**

#  Important Notes
- Space Complexity measures memory usage.
- Less memory means a better algorithm.
- Auxiliary Space does not include input memory.
- Constant memory is always preferred.

#  Memory Trick

Remember:
### **I + A = S**
```
I → Input Space
A → Auxiliary Space
S → Space Complexity
```

#  Interview Questions (Part 1)

### Basic
1. What is Space Complexity?
2. Why is Space Complexity important?
3. What is Input Space?
4. What is Auxiliary Space?
5. Write the formula of Space Complexity.
6. Which is better: O(1) or O(n) Space Complexity?

#  Summary (Part 1)
- Space Complexity measures memory usage.
- It consists of Input Space and Auxiliary Space.
- O(1) means constant memory.
- O(n) means memory increases with input size.
- Efficient algorithms use less memory.

# (Part-2)

# Table of Contents (Part 2)

1. Types of Space Complexity
2. Constant Space - O(1)
3. Linear Space - O(n)
4. Quadratic Space - O(n²)
5. Logarithmic Space - O(log n)
6. Time Complexity vs Space Complexity
7. Java Examples
8. Memory Diagrams
9. Important Notes
10. Interview Questions

---

# 7 Types of Space Complexity

Depending on the memory used, Space Complexity can be divided into different types.

```
          Space Complexity

                 │

     ┌───────────┼────────────┬────────────┐

     │           │            │            │

   O(1)        O(log n)      O(n)       O(n²)
```

---

# 1. Constant Space — O(1)

##  English
If the memory used by the algorithm remains constant regardless of the input size, then its Space Complexity is **O(1)**.

##  Hindi
Agar input kitna bhi bada ho, lekin memory same rahe, to Space Complexity **O(1)** hoti hai.

---

### Example

```java
int a = 10;
int b = 20;
int sum = a + b;
```

Only three variables are created.

Even if input increases,

memory remains the same.

Therefore,

```
Space Complexity = O(1)
```

#  Memory Diagram

```
+------+

a = 10

+------+

+------+

b = 20

+------+

+------+

sum = 30

+------+
```

---

# 2. Linear Space — O(n)

## English
If memory increases linearly with the input size, the Space Complexity is **O(n)**.

##  Hindi
Agar input badhne ke saath memory bhi badhti hai, to Space Complexity **O(n)** hoti hai.

---

### Example

```java
int arr[] = new int[n];
```

If

```
n = 10
```

Memory is required for 10 elements.

If

```
n = 100
```

Memory is required for 100 elements.

Hence,

```
O(n)
```

---

#  Memory Diagram

```
Input = 5

+----+----+----+----+----+

| | | | | |

+----+----+----+----+----+

5 Memory Blocks
```

---

# 3. Quadratic Space — O(n²)

## English

If memory grows as the square of the input size, the Space Complexity is **O(n²)**.

---

##  Hindi

Agar input ka square jitni memory lage, to Space Complexity **O(n²)** hoti hai.

---

### Example

```java
int matrix[][] = new int[n][n];
```

If

```
n = 5
```

Memory = 25 elements

If

```
n = 100
```

Memory = 10000 elements

# Memory Diagram

```
Matrix

□ □ □

□ □ □

□ □ □
```

# 4. Logarithmic Space — O(log n)

##  English
Some algorithms use memory that increases very slowly with input size.
This is called **O(log n)**.

##  Hindi
Kuch algorithms me input badhne ke baad bhi memory bahut kam badhti hai.
Isse **O(log n)** kehte hain.

### Example

Binary Search
Binary Search repeatedly divides the search space into two halves.
It requires very little extra memory.

# Real-Life Example

Imagine a library.

### O(1)

One bookmark.
No matter how many books are there,
you still use only one bookmark.

### O(n)

One bookmark for every book.
Books increase,
bookmarks also increase.

### O(n²)

One shelf for every book and every subject.
Memory grows very fast.

### O(log n)

Every time you divide books into half,

the memory requirement increases very slowly.

#  Time Complexity vs Space Complexity

| Time Complexity | Space Complexity |
|-----------------|------------------|
| Measures execution time | Measures memory usage |
| Faster is better | Less memory is better |
| Represented using Big-O | Represented using Big-O |

# Java Example

```java
public class Demo {

    public static void main(String[] args) {

        int[] arr = new int[5];

        int sum = 0;

        for(int i = 0; i < arr.length; i++) {

            sum += arr[i];

        }

        System.out.println(sum);

    }

}
```

### Analysis

Input Array

```
O(n)
```

Extra Variable

```
sum
↓
O(1)
```

Overall Space Complexity

```
O(n)
```

#  Important Notes

- O(1) is the most memory-efficient.
- O(n) is acceptable in many cases.
- O(n²) consumes large memory.
- Good algorithms balance both time and space.

#  Common Beginner Mistakes

* Confusing Time Complexity with Space Complexity.

* Counting input memory as auxiliary space.

* Assuming loops always increase Space Complexity.

*  Ignoring temporary variables.

#  Memory Trick

Remember:
```
O(1)
↓
Best
↓
O(log n)
↓
O(n)
↓
O(n²)
Worst
```

#  Interview Questions (Part 2)

### Basic
1. What is Constant Space?
2. What is Linear Space?
3. What is Quadratic Space?
4. Explain Logarithmic Space.
5. Which Space Complexity is best?

### Intermediate
1. Differentiate O(1) and O(n).
2. Explain O(n²) with an example.
3. Compare Time and Space Complexity.
4. Why is O(log n) considered efficient?
5. Give real-life examples of different Space Complexities.
6. 
#  Summary (Part 2)
- O(1) → Constant Memory
- O(log n) → Slowly Increasing Memory
- O(n) → Linear Memory
- O(n²) → Quadratic Memory
- Lower Space Complexity is generally preferred.

# (Part-3)
#  Important Definitions

## Space Complexity

###  English
Space Complexity is the total memory required by an algorithm during its execution.

### Hindi
Space Complexity kisi algorithm ko execute hone ke liye required total memory ko represent karti hai.

## Input Space

### English
Input Space is the memory required to store the input data.

### Hindi
Input Space woh memory hai jo input data ko store karne ke liye use hoti hai.

## Auxiliary Space

### English
Auxiliary Space is the extra memory used by an algorithm apart from the input.

### Hindi
Auxiliary Space algorithm dwara use ki gayi extra memory hoti hai jo input ka part nahi hoti.

## Constant Space
Memory remains the same even if the input size increases.

```
Space Complexity = O(1)
```

## Linear Space
Memory increases directly with the input size.

```
Space Complexity = O(n)
```

## Quadratic Space
Memory grows according to the square of the input size.

```
Space Complexity = O(n²)
```

## Logarithmic Space
Memory increases very slowly as the input size grows.

```
Space Complexity = O(log n)
```

#  Real-Life Example

Imagine a school examination.

### Input Space

Question Paper 

### Auxiliary Space

Rough Sheet 
The rough sheet is extra memory used to solve the questions.
Similarly,
Algorithms use Auxiliary Space to perform calculations.

#  Viva Questions

### Basic Viva

**Q1. What is Space Complexity?**
**Answer:** It is the total memory required by an algorithm during execution.

**Q2. What is Input Space?**
**Answer:** Memory used to store the input.

**Q3. What is Auxiliary Space?**
**Answer:** Extra memory used by an algorithm excluding the input.

**Q4. Which Space Complexity is best?**
**Answer:** O(1)

**Q5. Which Space Complexity uses the most memory among O(1), O(log n), O(n), and O(n²)?**
**Answer:** O(n²)

#  Interview Questions

## Beginner Level
1. What is Space Complexity?
2. Why is Space Complexity important?
3. What is Auxiliary Space?
4. Explain O(1) Space Complexity.
5. Explain O(n) Space Complexity.
6. Explain O(log n) Space Complexity.
7. Explain O(n²) Space Complexity.
8. What is the difference between Input Space and Auxiliary Space?

## Intermediate Level
1. Explain different types of Space Complexity with examples.
2. Compare O(1) and O(n).
3. Compare Time Complexity and Space Complexity.
4. Why is O(log n) considered efficient?
5. Can an algorithm have low Time Complexity but high Space Complexity? Explain.

#  MCQs

### Q1. Space Complexity measures:
- A. Execution Time
- B. Memory Usage.   (Correct)
- C. CPU Speed
- D. Network Speed

### Q2. Which Space Complexity is the best?
- A. O(1).      (Correct)
- B. O(n)
- C. O(n²)
- D. O(n³)

### Q3. Extra memory used by an algorithm is called:
- A. Input Space
- B. Auxiliary Space.  (Correct)
- C. Heap Space
- D. Stack Space

### Q4. Which algorithm commonly uses O(log n) extra space?
- A. Binary Search.  (Correct)
- B. Bubble Sort
- C. Linear Search
- D. Selection Sort

### Q5. An array of size `n` generally requires:
- A. O(1)
- B. O(n).      (Correct)
- C. O(log n)
- D. O(n²)

### Q6. Which notation is used to represent Space Complexity?
- A. Theta (Θ)
- B. Omega (Ω)
- C. Big-O (O).     (Correct)
- D. Sigma (Σ)

### Q7. Input Space + Auxiliary Space =
- A. Time Complexity
- B. Space Complexity    (Correct)
- C. Big-O
- D. Runtime

### Q8. Which statement is correct?
- A. Loops always increase Space Complexity.
- B. Loops do not always increase Space Complexity.    (Correct)
- C. Every algorithm has O(n²) Space Complexity.
- D. Space Complexity measures execution time.

### Q9. Which is more memory-efficient?
- A. O(1).    (Correct)
- B. O(n)
- C. O(n²)
- D. O(n³)

### Q10. Temporary variables are part of:
- A. Input Space
- B. Auxiliary Space.  (Correct)
- C. Output Space
- D. Cache Memory

#  Practice Questions

### Short Questions
1. Define Space Complexity.
2. What is Input Space?
3. What is Auxiliary Space?
4. Explain O(1) Space Complexity.
5. Explain O(n) Space Complexity.

### Long Questions
1. Explain Space Complexity with suitable examples.
2. Differentiate Input Space and Auxiliary Space.
3. Explain different types of Space Complexity.
4. Compare Time Complexity and Space Complexity.
5. Explain Space Complexity using memory diagrams.

#  Common Errors & Solutions

| Mistake | Reason | Correct Approach |
|----------|---------|------------------|
| Confusing Time with Space Complexity | Lack of understanding | Remember: Time = Execution Time, Space = Memory |
| Counting Input as Auxiliary Space | Wrong analysis | Count only extra memory as Auxiliary Space |
| Assuming loops always increase Space Complexity | Misconception | Loops affect time more than space in many cases |
| Ignoring temporary variables | Incomplete analysis | Count all extra variables used |

#  Exam Tips

* Learn the formula:

```
Space Complexity
=
Input Space
+
Auxiliary Space
```

* Remember the order:

```
Best
↓
O(1)
↓
O(log n)
↓
O(n)
↓
O(n²)
↓
Worst
```

#  Chapter Summary
- Space Complexity measures memory usage.
- It consists of Input Space and Auxiliary Space.
- O(1) uses constant memory.
- O(log n) uses slowly increasing memory.
- O(n) uses memory proportional to input.
- O(n²) uses quadratic memory.
- Lower Space Complexity is generally preferred.


# Chapter Sheet

```
Space Complexity

        │

Input Space

        +

Auxiliary Space

        │

        ▼

Total Memory Used
```

### Memory Ranking

```
Best
↓
O(1)
↓
O(log n)
↓
O(n)
↓
O(n²)
↓
Worst
```

<div align="center">

#  Chapter 04 Completed Successfully!

> **"A good programmer not only writes fast algorithms but also writes memory-efficient algorithms."**

⭐ Happy Learning & Keep Coding! ⭐

</div>