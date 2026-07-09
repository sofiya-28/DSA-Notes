#  Chapter 3: Time Complexity 
# (Part-1)

# Table of Contents (Part 1)

1. What is Time Complexity?
2. Why Do We Need Time Complexity?
3. Real-Life Example
4. Time vs Running Time
5. Algorithm
6. Input Size (n)
7. Why Not Measure Time in Seconds?
8. Memory Diagram
9. Interview Questions
10. Quick Revision

# What is Time Complexity?

## English
Time Complexity is a way to measure **how the execution time of an algorithm grows as the input size increases**.
It does **NOT** measure the exact time in seconds.
Instead, it tells us how fast or slow an algorithm grows when the amount of data becomes larger.
## 🇮🇳 Hindi
Time Complexity batati hai ki **jaise-jaise input size (n) badhta hai, waise-waise kisi algorithm ko complete hone me kitna time lagega.**
Ye **seconds ya milliseconds** nahi batati.
Ye sirf batati hai ki algorithm data badhne par kitna efficient hai.

#  Simple Definition (Exam)
**Time Complexity** is the measurement of the amount of time an algorithm takes with respect to the input size.

#  Real-Life Example
Imagine you have to find your friend in a classroom.
### Case 1
There are only **5 students**.
Finding your friend is easy.

### Case 2
Now imagine there are **500 students**.
It will take more time.

### Case 3
Now imagine there are **50,000 students**.
Finding your friend becomes much harder.
This shows that **as input size increases, execution time also changes.**
That relationship is called **Time Complexity.**

#  Visual Diagram

```
Small Input (5)
      │
      ▼
Less Time

--------------------------

Medium Input (500)
      │
      ▼
More Time

--------------------------

Large Input (50,000)
      │
      ▼
Much More Time
```

---

# Why Do We Need Time Complexity?
Suppose two students write the same program.
Student A
```
Search Time = 2 seconds
```

Student B
```
Search Time = 10 seconds
```
Does this always mean Student A's algorithm is better?  No  (Why?)
Because:
- Different Computers
- Different CPUs
- Different RAM
- Different Operating Systems

all affect actual execution time.

Therefore,
Computer time is **not a reliable way** to compare algorithms.
Instead, we compare how algorithms grow as input size increases.
That is Time Complexity.

#  Real-Life Example

Imagine
Person A rides a Bicycle.
Person B rides a Bike.
Person C rides a Car.
If the road changes,
their speed changes.
Similarly,
Different computers give different execution times.
Therefore,
We compare algorithms mathematically instead of comparing seconds.

#  Running Time vs Time Complexity

Many beginners think these are the same.
They are NOT.

| Running Time | Time Complexity |
|--------------|-----------------|
| Measured in Seconds | Measured using Mathematical Growth |
| Depends on Computer | Independent of Computer |
| Changes on Different Systems | Same Everywhere |

#  What is an Algorithm?

##  English
An Algorithm is a **step-by-step procedure** used to solve a problem.
## 🇮🇳 Hindi
Algorithm kisi problem ko solve karne ke liye **step-by-step instructions** ka set hota hai.

#  Example Algorithm
Problem:
Make Tea

Algorithm:

```
Start
↓
Boil Water
↓
Add Tea Leaves
↓
Add Sugar
↓
Add Milk
↓
Boil
↓
Serve Tea
↓
End

```
Every program follows some algorithm.

#  What is Input Size (n)?

Input Size means
**How much data is given to the algorithm.**
We represent it by

```
n
```

Example

```
n = 10

10 numbers
```

```
n = 100

100 numbers
```

```
n = 1,000,000

One Million Numbers
```

As **n increases**, Time Complexity becomes more important.

# Input Size Diagram

```
n = 5

⬜⬜⬜⬜⬜

--------------------

n = 100

⬜⬜⬜⬜⬜⬜⬜⬜⬜⬜....

--------------------

n = 100000

Huge Amount of Data
```

#  Why Don't We Measure Time in Seconds?
Because:
✔ Different CPU
✔ Different RAM
✔ Different Operating System
✔ Different Programming Language
✔ Different Compiler
can produce different execution times.
Therefore,
Time Complexity is measured mathematically.

# Memory Trick

Remember

```
Time Complexity
=
Growth of Time
NOT
Actual Time

```
#  Interview Questions

## Basic
1. What is Time Complexity?
2. Why do we need Time Complexity?
3. What is an Algorithm?
4. What is Input Size?
5. Why don't we measure execution time in seconds?

## Intermediate
1. Difference between Running Time and Time Complexity.
2. Explain Time Complexity with a real-life example.

# Common Mistakes
Wrong:     Time Complexity tells exact seconds.
Right:     Time Complexity only shows the growth of execution time.

Wrong:     Faster computer means better algorithm.
Right:     A good algorithm is determined by its Time Complexity, not by computer speed.

#  Quick Revision
✔ Time Complexity studies algorithm growth.
✔ It depends on Input Size (n).
✔ It does not measure exact seconds.
✔ Algorithm = Step-by-step solution.
✔ Running Time ≠ Time Complexity.

#  Summary
- Time Complexity measures how an algorithm grows as input size increases.
- It is independent of hardware.
- It helps compare algorithms fairly.
- Input size is represented by **n**.
- Algorithms are compared mathematically, not by stopwatch.
# (Part-2)

# Part-2 Big O Notation & Types of Time Complexity

In this part, we will learn:
* What is Big O Notation?
* Why Big O is used?
* Types of Time Complexity
* Best, Average and Worst Case

#  What is Big O Notation?

##  English
Big O Notation is a mathematical way to describe the performance of an algorithm as the input size increases.
It tells us how efficiently an algorithm works for large amounts of data.

## 🇮🇳 Hindi
Big O Notation ek mathematical notation hai jo batati hai ki input size badhne par algorithm ki performance kaise change hoti hai.
Ye algorithm ki efficiency ko represent karti hai.

# Simple Definition (Exam)
**Big O Notation is used to represent the Time Complexity of an algorithm.**

#  Why Do We Use Big O?
Suppose we have two algorithms.

Algorithm A
```
100 Operations
```

Algorithm B
```
1000 Operations
```

Which one is better?
Obviously,
Algorithm A
because it performs fewer operations.
Big O helps us compare algorithms.

#  Real-Life Example
Imagine two students searching for a book.
Student A checks every book one by one.
Student B goes directly to the correct shelf using the catalogue.
Student B finishes much faster.
Big O helps compare both methods.

# Types of Time Complexity
There are three cases.

```
Best Case
↓
Average Case
↓
Worst Case
```

#  Best Case

## English
The minimum time taken by an algorithm.
Everything happens perfectly.

## 🇮🇳 Hindi
Algorithm ko problem solve karne ke liye sabse kam time lage.

## Example
Searching number 50.
Array

```
50 20 30 40 10
```
50 is found immediately.
Best Case.

# Average Case

## English
The expected time taken for a normal input.

## 🇮🇳 Hindi
Generally algorithm jitna time leta hai.
Na bahut fast
Na bahut slow.

##  Example

Searching 40
```
10 20 30 40 50
```
Need to check some elements first.
Average Case.

#  Worst Case

## English
The maximum time taken by an algorithm.

## 🇮🇳 Hindi
Algorithm ko sabse zyada time lagta hai.

## Example
Searching 50
```
10 20 30 40 50
```
Suppose algorithm checks every element before reaching 50.
Worst Case.

#  Best vs Average vs Worst

| Case | Meaning | Time |
|------|---------|------|
| Best | Minimum Time | Fastest |
| Average | Normal Time | Medium |
| Worst | Maximum Time | Slowest |

#  Visual Representation

```
Best Case
↓
Average Case
↓
Worst Case
```

# Why Do Interviews Focus on Worst Case?
Because:
Worst Case guarantees the maximum time an algorithm can take.
Interviewers usually ask for Worst Case Time Complexity.

# Memory Trick
Remember:

```
Best
↓
Average
↓
Worst
Fast
↓
Normal
↓
Slow
```

#  Interview Questions

## Basic
1. What is Big O Notation?
2. Why do we use Big O?
3. What are the three cases of Time Complexity?
4. Which case is mostly used in interviews?

## Intermediate
1. Explain Best, Average and Worst Case with examples.
2. Why is Worst Case preferred over Best Case?

#  MCQs

### Q1. Big O Notation represents:
A. Memory
B. CPU Speed
C. Time Complexity     (Correct)
D. RAM Size

### Q2. Which case represents maximum execution time?
A. Best
B. Average
C. Worst   (Correct)
D. Minimum

### Q3. Which case is mostly discussed in interviews?
A. Best
B. Average
C. Worst   (Correct)
D. None

#  Practice Questions
1. Define Big O Notation.
2. Why is Big O important?
3. Explain Best Case with an example.
4. Explain Average Case.
5. Explain Worst Case.
6. Why do interviewers prefer Worst Case?

#  Quick Revision
* Big O → Mathematical representation of Time Complexity.
* Best Case → Minimum Time.
* Average Case → Normal Time.
* Worst Case → Maximum Time.
* Interviews mainly focus on Worst Case.

#  Summary
- Big O Notation measures algorithm efficiency.
- It helps compare different algorithms.
- Time Complexity has three cases: Best, Average and Worst.
- Worst Case is the most important in coding interviews.

# (Part-3)

# Part 3: Common Time Complexities

In this section, we will learn the four most important time complexities asked in interviews.

- O(1)
- O(log n)
- O(n)
- O(n log n)

# 1️ O(1) - Constant Time Complexity
##  English
An algorithm takes the **same amount of time**, no matter how large the input size is.
The execution time never changes.

## 🇮🇳 Hindi
Chahe input me 10 elements ho ya 10 lakh elements, algorithm hamesha same time lega.
Isliye ise **Constant Time Complexity** kehte hain.

##  Example

Accessing an element of an array using its index.
```java
int[] arr = {10,20,30,40,50};
System.out.println(arr[2]);
```
Output:
```
30
```
No matter how big the array is, accessing index 2 always takes almost the same time.


## Diagram

```
Input Size
10
100
1000
100000
↓
Time
1 Step
1 Step
1 Step
1 Step
```
---

##  Real-Life Example
Imagine you know your friend's roll number.
Teacher directly tells where your friend sits.
No searching required.

# 2️ O(log n) - Logarithmic Time Complexity

##  English
The algorithm reduces the search space by half in every step.
This is much faster than checking every element.

## 🇮🇳 Hindi
Har step me data aadha ho jata hai.
Isliye algorithm bahut fast hota hai.

##  Example

Binary Search
Suppose
```
100 Numbers
```

Step 1
↓
50
↓
25
↓
12
↓
6
↓
3
↓
1
Only a few steps are needed.

##  Diagram

```
100
↓
50
↓
25
↓
12
↓
6
↓
3
↓
1
```

## Real-Life Example
Dictionary me word search karna.
Har page nahi dekhte.
Beech se start karte hain.

##  Used In
✔ Binary Search
✔ Balanced Trees
✔ Divide and Conquer

# 3️ O(n) - Linear Time Complexity

##  English
The algorithm checks every element one by one.
Time increases directly with input size.

## 🇮🇳 Hindi
Jitna input badhega utna hi algorithm ka time badhega.

##  Java Example

```java
int[] arr={10,20,30,40,50};

for(int i=0;i<arr.length;i++)
{
    System.out.println(arr[i]);
}
```
The loop visits every element once.

##  Diagram
```
n = 5
*****
5 Steps
--------------
n = 100
************************
100 Steps
```

## Real-Life Example
Attendance checking.
Teacher checks every student one by one.

# 4️ O(n log n)

##  English
This complexity is better than O(n²).
Many efficient sorting algorithms use O(n log n).

## 🇮🇳 Hindi
Ye complexity Linear se thodi slow aur Quadratic se bahut fast hoti hai.
Sorting algorithms me ye bahut common hai.

##  Examples
✔ Merge Sort
✔ Heap Sort
✔ Quick Sort (Average Case)

## Diagram
```
n
×
log n
↓
O(n log n)
```

##  Real-Life Example
Imagine a teacher divides the class into groups and then checks every group efficiently.
This saves a lot of time compared to checking randomly.

# Comparison Table

| Complexity | Name | Speed | Example |
|------------|------|-------|---------|
| O(1) | Constant | ⭐⭐⭐⭐⭐ | Array Index |
| O(log n) | Logarithmic | ⭐⭐⭐⭐ | Binary Search |
| O(n) | Linear | ⭐⭐⭐ | Linear Search |
| O(n log n) | Efficient | ⭐⭐⭐⭐ | Merge Sort |

# Performance Graph

```
Time

│
│                  O(n log n)
│              /
│           /
│        O(n)
│      /
│   O(log n)
│  /
│ O(1)
│___________________________ Input Size
```

#  Interview Questions

1. What is O(1)?
2. Give one example of O(log n).
3. Why is Binary Search O(log n)?
4. Why is Linear Search O(n)?
5. Which is better: O(n) or O(n log n)?

# MCQs

### Q1. Accessing an array element by index has:
A. O(n)
B. O(log n)
C. O(1)      (Correct)
D. O(n²)

### Q2. Binary Search has:
A. O(n)
B. O(n²)
C. O(log n)     (Correct)
D. O(1)

### Q3. Merge Sort has:
A. O(n²)
B. O(1)
C. O(n)
D. O(n log n)    (Correct)

#  Practice Questions
1. Explain O(1) with an example.
2. Explain O(log n) using Binary Search.
3. Why is Linear Search O(n)?
4. Compare O(1), O(log n), O(n) and O(n log n).
5. Draw the Time Complexity graph.

#  Quick Revision
* O(1) → Constant
* O(log n) → Binary Search
* O(n) → Linear Search
* O(n log n) → Merge Sort

# (part-4)

# Part 4: O(n²), O(2ⁿ), O(n!), Space Complexity & Time vs Space Complexity

In this part, we will learn:
* O(n²)
* O(2ⁿ)
* O(n!)
* Space Complexity
* Time Complexity vs Space Complexity

# 1️ O(n²) - Quadratic Time Complexity

##  English
An algorithm has **O(n²)** time complexity when it uses **two nested loops**.
As the input size increases, the number of operations increases very quickly.

## 🇮🇳 Hindi
Jab kisi program me **nested loops (loop ke andar loop)** use hote hain, to uski Time Complexity aksar **O(n²)** hoti hai.
Input double hone par operations lagbhag 4 times ho jate hain.

## Java Example

```java
for(int i = 0; i < n; i++)
{
    for(int j = 0; j < n; j++)
    {
        System.out.println(i + " " + j);
    }
}
```
Time Complexity
```
O(n²)
```

## Real-Life Example

Imagine every student shakes hands with every other student.
If there are more students, handshakes increase very quickly.

## Examples
✔ Bubble Sort
✔ Selection Sort
✔ Matrix Traversal

# 2️ O(2ⁿ) - Exponential Time Complexity

##  English
In **O(2ⁿ)**, the number of operations doubles with each increase in input size.
This becomes very slow for large inputs.

## 🇮🇳 Hindi
Har naye input ke saath operations lagbhag double ho jate hain.
Isliye ye large inputs ke liye practical nahi hoti.


##  Example

```
n = 1 → 2
n = 2 → 4
n = 3 → 8
n = 4 → 16
n = 5 → 32
```
## Used In
✔ Recursive Problems
✔ Backtracking (Without Optimization)

# 3️ O(n!) - Factorial Time Complexity

## English
This is one of the slowest time complexities.
The algorithm tries every possible arrangement.

## 🇮🇳 Hindi
Algorithm har possible arrangement ko check karta hai.
Input thoda sa badhne par bhi operations bahut zyada ho jate hain.

##  Example
Finding all possible arrangements of people.

```
3 People
ABC
ACB
BAC
BCA
CAB
CBA
```
Total
```
3! = 6
```

## Used In

✔ Permutations
✔ Travelling Salesman Problem (Brute Force)

#  Complexity Comparison Table

| Complexity | Name | Speed | Example |
|------------|------|-------|---------|
| O(1) | Constant | ⭐⭐⭐⭐⭐ | Array Index |
| O(log n) | Logarithmic | ⭐⭐⭐⭐ | Binary Search |
| O(n) | Linear | ⭐⭐⭐ | Linear Search |
| O(n log n) | Linearithmic | ⭐⭐⭐⭐ | Merge Sort |
| O(n²) | Quadratic | ⭐⭐ | Bubble Sort |
| O(2ⁿ) | Exponential | ⭐ | Recursion |
| O(n!) | Factorial | ⭐ | Permutations |

# Complexity Growth Graph

```
Time

│                                 O(n!)
│                            /
│                        O(2ⁿ)
│                     /
│                 O(n²)
│              /
│          O(n log n)
│        /
│     O(n)
│   /
│ O(log n)
│/
O(1)
└──────────────────────────────► Input Size
```

# What is Space Complexity?
## English
Space Complexity measures the amount of memory required by an algorithm during execution.

## 🇮🇳 Hindi
Space Complexity batati hai ki algorithm ko execute hone ke liye kitni memory chahiye.

## Java Example
```java
int a = 10;
int b = 20;
int sum = a + b;
```

Only a few variables are used.

Space Complexity
```
O(1)
```

# Real-Life Example
Imagine you are travelling.
Small backpack  → Less Space
Big suitcase  → More Space
Similarly,
Less Memory → Better Space Complexity

# Time Complexity vs Space Complexity

| Time Complexity | Space Complexity |
|-----------------|------------------|
| Measures execution time | Measures memory usage |
| Focuses on speed | Focuses on storage |
| Written using Big O | Also written using Big O |

#  Which is More Important?
There is no single answer.
Sometimes
* Faster algorithm is preferred.
Sometimes
* Lower memory usage is preferred.
It depends on the problem.

# Interview Questions

## Basic
1. What is O(n²)?
2. Give one example of O(2ⁿ).
3. What is O(n!)?
4. What is Space Complexity?
5. Difference between Time and Space Complexity.

## Intermediate
1. Why is Bubble Sort O(n²)?
2. Which is worse: O(2ⁿ) or O(n!)?
3. Can an algorithm have good Time Complexity but poor Space Complexity?

#  MCQs
### Q1. Two nested loops usually have
A. O(n)
B. O(n²)    (Correct)
C. O(log n)
D. O(1)

### Q2. Bubble Sort worst-case complexity is
A. O(log n)
B. O(n)
C. O(n²)   (Correct)
D. O(1)

### Q3. Space Complexity measures
A. CPU Speed
B. Input Size
C. Memory Usage    (Correct)
D. Internet Speed

### Q4. Which is the slowest?
A. O(1)
B. O(log n)
C. O(n)
D. O(n!)           (Correct)

# Practice Questions

1. Explain O(n²) with an example.
2. Why is O(2ⁿ) inefficient?
3. Explain O(n!).
4. Define Space Complexity.
5. Compare Time Complexity and Space Complexity.

# Quick Revision
* O(n²) → Nested Loops
* O(2ⁿ) → Exponential Growth
* O(n!) → Factorial Growth
* Space Complexity → Memory Usage
* Time Complexity → Execution Time

#  Summary
- O(n²) usually appears with nested loops.
- O(2ⁿ) grows exponentially and becomes slow quickly.
- O(n!) is one of the slowest complexities.
- Space Complexity measures memory usage.
- A good algorithm tries to balance both Time and Space Complexity.

---

# Part 5: (Overall Revision)

# One Page Sheet

| Complexity | Name | Common Example |
|------------|------|----------------|
| O(1) | Constant | Array Index Access |
| O(log n) | Logarithmic | Binary Search |
| O(n) | Linear | Linear Search |
| O(n log n) | Linearithmic | Merge Sort |
| O(n²) | Quadratic | Bubble Sort |
| O(2ⁿ) | Exponential | Recursive Problems |
| O(n!) | Factorial | Permutations |


# Complexity Ranking (Best → Worst)
```
O(1)
↓
O(log n)
↓
O(n)
↓
O(n log n)
↓
O(n²)
↓
O(2ⁿ)
↓
O(n!)
```

> The higher you go in this list, the better the algorithm.


#  Memory Tricks

## Trick 1
Remember this order
```
1
↓
log n
↓
n
↓
n log n
↓
n²
↓
2ⁿ
↓
n!
```

## Trick 2
Fastest
O(1)

Slowest
O(n!)

## Trick 3
Nested Loop
↓
Always think
```
O(n²)
```

## Trick 4
Binary Search
↓
Always remember
```
O(log n)
```

#  Most Asked Interview Questions

## Basic Level
1. What is Time Complexity?
2. Why do we use Big O?
3. Difference between Time and Space Complexity?
4. Why is Binary Search O(log n)?
5. Why is Linear Search O(n)?

## Intermediate Level
1. Explain O(n log n).
2. Why is Merge Sort better than Bubble Sort?
3. Which Time Complexity is best?
4. Which Time Complexity is worst?
5. Explain O(2ⁿ).

## Advanced Level
1. How do you calculate Time Complexity?
2. Can an algorithm have multiple Time Complexities?
3. Why do interviews prefer Worst Case Complexity?
4. Can Time Complexity be reduced?
5. Is lower Time Complexity always better?

# Final MCQs

### Q1
The best Time Complexity is
A. O(n²)
B. O(n)
C. O(log n)
D. O(1)         (Correct)

### Q2
Binary Search works in
A. O(n)
B. O(n²)
C. O(log n)      (Correct)
D. O(1)

### Q3
Bubble Sort Worst Case
A. O(log n)
B. O(n)
C. O(n²)        (Correct)
D. O(1)

### Q4
Which complexity grows the fastest?
A. O(n)
B. O(log n)
C. O(n²)
D. O(n!)       (Correct)

### Q5
Space Complexity measures
A. CPU Speed
B. Internet Speed
C. Memory Usage      (Correct)
D. Input Size

#  Practice Questions

## Easy
1. Define Time Complexity.
2. Define Big O.
3. Define Space Complexity.
4. Explain O(1).
5. Explain O(n).

## Medium
1. Compare O(log n) and O(n).
2. Compare O(n²) and O(n log n).
3. Explain Worst Case.
4. Explain Best Case.
5. Explain Average Case.

## Hard
1. Compare all Time Complexities.
2. Explain Complexity Growth Graph.
3. Explain why O(1) is the fastest.
4. Explain why O(n!) is the slowest.
5. Explain Time Complexity with real-life examples.

#  Interview Tips
✔ Always mention Big O Notation.
✔ Explain with a real-life example.
✔ Draw a small graph if possible.
✔ Compare algorithms instead of memorizing formulas.
✔ Remember common examples:
O(1) → Array Index
O(log n) → Binary Search
O(n) → Linear Search
O(n²) → Bubble Sort

#  Quick Revision
* Time Complexity → Growth of execution time
* Space Complexity → Memory usage
* Big O → Mathematical notation
* Binary Search → O(log n)
* Linear Search → O(n)
* Merge Sort → O(n log n)
* Bubble Sort → O(n²)

#  Chapter Summary

After completing this chapter, you have learned:
✔ Time Complexity
✔ Big O Notation
✔ Best, Average & Worst Case
✔ O(1)
✔ O(log n)
✔ O(n)
✔ O(n log n)
✔ O(n²)
✔ O(2ⁿ)
✔ O(n!)
✔ Space Complexity
✔ Time vs Space Complexity
✔ Interview Questions
✔ MCQs
✔ Practice Questions

Congratulations! 
You have successfully completed **Chapter 3 - Time Complexity**.

----