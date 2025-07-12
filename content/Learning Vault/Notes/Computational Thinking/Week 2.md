# WEEK 2: Iteration, Filtering, Selection, Pseudocode, Finding Max and Min, AND Operator

This week introduces the core control flow constructs that allow algorithms to perform repetitive tasks and make decisions. These are fundamental for any program.

## 2.1 Iteration (Loops)

*   **Definition:** A control flow construct that allows a block of code to be executed repeatedly until a certain condition is met. Essential for processing collections of data.
*   **Pseudocode Constructs:**
    *   `while (condition is true) { ... }`: The loop continues as long as the condition remains true. It's crucial to have something inside the loop that *eventually* makes the condition false, or it will be an **infinite loop**.
    *   **Processing Data from Tables (Common Pattern):**
        ```pseudocode
        while (Table has more rows) {
          Read the first row X from Table
          // Process X
          Move X to another table // This typically makes the "Table has more rows" condition eventually false
        }
        ```
    *   **Accumulators/Counters within loops:** Variables often initialized to 0 (for sums or counts) or a sentinel value (for max/min) and updated in each iteration.

## 2.2 Filtering and Selection (Conditionals)

*   **Definition:** Mechanisms for executing different blocks of code based on whether a condition is true or false.
*   **Pseudocode Constructs:**
    *   `if (condition) { ... }`: Executes the block only if the condition is true.
    *   `if (condition) { ... } else { ... }`: Executes one block if true, another if false.
    *   `if (condition 1) { ... } else if (condition 2) { ... } else { ... }`: For multiple mutually exclusive conditions.

## 2.3 Logical Operators

*   **AND (`&&` or `and`):**
    *   **Definition:** Combines two or more conditions. The entire combined condition is `True` only if *all* individual conditions are `True`.
    *   **Truth Table:**
        | Condition 1 | Condition 2 | Result (C1 AND C2) |
        | :---------- | :---------- | :----------------- |
        | True        | True        | True               |
        | True        | False       | False              |
        | False       | True        | False              |
        | False       | False       | False              |
*   **OR (`||` or `or`):** (Introduced in Week 3, but related)
    *   **Definition:** Combines two or more conditions. The entire combined condition is `True` if *at least one* individual condition is `True`.
*   **NOT (`!` or `not`):**
    *   **Definition:** Inverts the truth value of a condition (`True` becomes `False`, `False` becomes `True`).

## 2.4 Pseudocode

*   **Definition:** An informal high-level description of the operating principle of a computer algorithm or other process. It uses plain language and programming-like constructs but is not executable code.
*   **Purpose:** To plan algorithms, communicate logic clearly, and bridge the gap between human language and programming language.
*   **Key Characteristics:**
    *   Uses keywords like `while`, `if`, `else`, `return`.
    *   Uses indentation to show block structure.
    *   Uses descriptive variable names.
    *   Abstracts away syntax details (e.g., `Read the first row X`, `Move X to Table 2`).

## 2.5 Finding Max and Min Values

*   **Technique:**
    1.  **Initialize a variable** (e.g., `max_val`, `min_val`) to a suitable starting value.
        *   For `max_val`: Initialize to a very small number (or the first element in the list).
        *   For `min_val`: Initialize to a very large number (or the first element in the list).
    2.  **Iterate** through the collection of data.
    3.  **Use a conditional (`if` statement)** to compare each new element with the current `max_val` or `min_val`.
    4.  **Update** `max_val` or `min_val` if a new extreme value is found.

---

**Common PYQ Pattern: Pseudocode Tracing & Logic Analysis (Fundamental)**
This is arguably the most common and important pattern. You're given pseudocode and asked to determine its output, what a variable represents, or what the procedure computes. It requires meticulous step-by-step execution.

**Example Question (Based on PYQ 6, July 2024 QDF4):**

The following pseudocode is executed using the "Scores" dataset. What will `A` represent at the end of the execution?

```pseudocode
1 A = 0
2 while(Pile 1 has more cards) {
3   Read the top card x from Pile 1
4   A = A + isInSeq(X)
5   Move X to Pile 2
6 }
7 Procedure isInSeq(X)
8   if(X.Physics < X.Mathematics){
9     if(X.Mathematics < X.Chemistry) {
10      return(1)
11    }
12  }
13  return (0)
14 End isInseq
```

**Options:**

- Number of students with highest marks in Chemistry and lowest marks in Physics. (Correct)
    
- Number of students with highest marks in Mathematics and lowest marks in Physics.
    
- Number of students with highest marks in Physics among the three subjects.
    
- Number of students with lowest marks in Physics and highest marks in Mathematics.
    

**Step-by-Step Solution:**

1. **Understand the Main Goal (A):**
    
    - Line 1: A = 0 (initializes a counter).
        
    - Lines 2-6 (main loop): Iterates through each student's record (X) in Pile 1. For each student, it calls isInSeq(X) and adds the returned value (either 0 or 1) to A. Move X to Pile 2 means each student is processed once.
        
    - **Conclusion for A's role:** A will count how many times the isInSeq procedure returns 1.
        
2. **Understand isInSeq(X) Procedure (The Core Logic):**
    
    - Line 7: This procedure takes a student's record X (which has Physics, Mathematics, Chemistry marks).
        
    - Line 8: if(X.Physics < X.Mathematics) - Checks if Physics score is less than Mathematics score.
        
    - Line 9: if(X.Mathematics < X.Chemistry) - This is a **nested if**. It's only checked IF the first condition (Physics < Mathematics) is true. It checks if Mathematics score is less than Chemistry score.
        
    - Line 10: return(1) - This line is reached **ONLY IF BOTH conditions are true**: X.Physics < X.Mathematics **AND** X.Mathematics < X.Chemistry.
        
    - Line 13: return(0) - If either of the conditions (or both) are false, this line is executed, and the procedure returns 0.
        
3. **Combine the Logic:**
    
    - isInSeq(X) returns 1 if a student's scores follow this specific sequence: Physics < Mathematics < Chemistry.
        
    - If Physics < Mathematics < Chemistry, this means:
        
        - Physics is the lowest score among the three.
            
        - Chemistry is the highest score among the three.
            
    - A counts how many students satisfy this specific condition.
        
4. **Match with Options:**
    
    - "Number of students with highest marks in Chemistry and lowest marks in Physics." - This accurately describes the condition Physics < Mathematics < Chemistry. If Physics is the lowest and Chemistry is the highest, then this condition is met.
        

**Final Answer:** A represents the number of students with highest marks in Chemistry and lowest marks in Physics.


