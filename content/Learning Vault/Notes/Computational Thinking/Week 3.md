

# WEEK 3: Multiple Iterations (Non-nested), Three Prizes Problem, Procedures, Parameters, Side Effects, OR Operator

This week builds on basic control flow by introducing more complex looping scenarios, the fundamental concept of reusable code blocks (procedures), and another key logical operator.

## 3.1 Multiple Iterations (Non-nested)

*   **Definition:** Using several independent loops in sequence. One loop finishes entirely before the next one begins.
*   **Purpose:** To perform distinct processing stages on the same (or different) datasets. For example, one loop to calculate a sum, then a second loop to process elements based on that sum.
*   **Contrast with Nested Iterations (Week 4):** Non-nested loops run sequentially, processing each item once per loop. Nested loops involve an inner loop completing all its iterations for *each* iteration of an outer loop, leading to $N \times M$ operations.

## 3.2 Procedures (Functions)

*   **Definition:** A self-contained block of code designed to perform a specific task. Also often called a "function" (especially if it returns a value) or "subroutine."
*   **Pseudocode Structure:**
    ```pseudocode
    Procedure ProcedureName (Parameter1, Parameter2, ...)
      // Code to perform the task
      return (Value) // Optional, if the procedure computes and returns a result
    End ProcedureName
    ```
*   **Calling a Procedure:** `Result = ProcedureName(Argument1, Argument2)`
*   **Benefits:**
    *   **Modularity:** Breaks down a large problem into smaller, manageable sub-problems.
    *   **Reusability:** The same procedure can be called multiple times from different parts of the code.
    *   **Readability:** Makes code easier to understand and maintain.

## 3.3 Parameters and Arguments

*   **Parameters:** Variables declared in the procedure's definition that act as placeholders for values that will be passed into the procedure when it's called.
*   **Arguments:** The actual values passed to a procedure when it is called. These values are assigned to the parameters.
*   **Example:** In `Procedure DoSomething(B)`, `B` is a parameter. When `DoSomething(10)` is called, `10` is the argument, and `B` inside the procedure will take the value 10.

## 3.4 Side Effects

*   **Definition:** When a procedure (or any block of code) modifies something outside its local scope, such as:
    *   Changing a global variable.
    *   Modifying an input parameter (if passed by reference).
    *   Performing input/output operations (e.g., printing to screen, writing to a file).
*   **Importance:** Can make code harder to debug and understand because a change in one part of the program might have unexpected consequences elsewhere. In functional programming, minimizing side effects is a key principle.

## 3.5 OR Operator

*   **Definition:** A logical operator that combines two or more conditions. The entire combined condition is `True` if *at least one* individual condition is `True`. It's only `False` if *all* individual conditions are `False`.
*   **Truth Table:**
    | Condition 1 | Condition 2 | Result (C1 OR C2) |
    | :---------- | :---------- | :---------------- |
    | True        | True        | True              |
    | True        | False       | True              |
    | False       | True        | True              |
    | False       | False       | False             |
*   **Contrast with AND:** `AND` is stricter (all true), `OR` is more permissive (any true).

---

**Common PYQ Pattern: Pseudocode Tracing (with Procedures & Max/Min logic)**
Tracing involves running the code mentally (or on paper) line by line, keeping track of variable values. Questions often involve finding max/min or cumulative values using loops and conditionals.

**Example Question (Based on PYQ 5, July 2024 QDF4):**

The given pseudocode is executed using "Scores" dataset. Let `B` be a positive integer. What does the procedure `DoSomething` compute?

```pseudocode
1 Procedure DoSomething (B)
2   C = 0, D = 101
3   while(Table 1 has more rows) {
4     Read the first row X in Table 1
5     if(X.Physics > C){
6       C = X.Physics
7     }
8     if(X.Chemistry < D){
9       D = X.Chemistry
10    }
11    Move X to Table 2
12  }
13  if(C - D >= B) {
14    return (False)
15  }
16  else{
17    return (True)
18  }
19 End DoSomething
```

**Options:**

- Returns “True” if and only if the difference between the maximum Physics marks and the minimum Chemistry marks is at least B
    
- Returns "True” if and only if the difference between the maximum Chemistry marks and the minimum Physics marks is at most B
    
- Returns "True" if and only if the difference between the maximum Physics marks and the minimum Chemistry marks is less than B (Correct)
    
- Returns "True” if and only if the difference between the maximum Chemistry marks and the minimum Physics marks is less than B
    

**Step-by-Step Solution:**

1. **Analyze Initialization (Line 2):**
    
    - C = 0: C is a variable designed to find a **maximum value**. Starting at 0 ensures any positive score will be greater and update C.
        
    - D = 101: D is a variable designed to find a **minimum value**. Starting at 101 (assuming marks out of 100) ensures any valid score will be smaller and update D.
        
2. **Analyze the Loop (Lines 3-12):**
    
    - while(Table 1 has more rows): This loop processes every student's record (X) in the "Scores" dataset. Move X to Table 2 ensures all records are processed once.
        
    - if(X.Physics > C) { C = X.Physics } (Lines 5-7): Inside the loop, C is continuously updated to the highest Physics mark encountered so far. At the end of the loop, C will hold the **Maximum Physics Mark** from the entire dataset.
        
    - if(X.Chemistry < D) { D = X.Chemistry } (Lines 8-10): Similarly, D is continuously updated to the lowest Chemistry mark encountered so far. At the end of the loop, D will hold the **Minimum Chemistry Mark** from the entire dataset.
        
3. **Analyze the Final Decision (Lines 13-18):**
    
    - After the loop, C = Max Physics Mark and D = Min Chemistry Mark.
        
    - if(C - D >= B) (Line 13): This checks if the difference between Max Physics and Min Chemistry is greater than or equal to B.
        
        - If TRUE, return (False).
            
    - else { return (True) } (Lines 16-17): If the condition (C - D >= B) is FALSE, it means (C - D < B).
        
        - If FALSE, return (True).
            
4. **Combine and Conclude:**  
    The procedure DoSomething(B) returns True if and only if (Max Physics Mark - Min Chemistry Mark) is strictly less than B.
    
5. **Match with Options:**
    
    - Only "Returns "True" if and only if the difference between the maximum Physics marks and the minimum Chemistry marks is less than B" matches our conclusion.
        

**Final Answer:** The procedure returns "True" if and only if the difference between the maximum Physics marks and the minimum Chemistry marks is less than B.



