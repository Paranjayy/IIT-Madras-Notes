# Week 1: Variables, Initialization, Iterators, Filtering, Datatypes, Flowcharts, Sanity of data

*   **Variables:** Named storage locations for data.
*   **Datatypes:** Classify data: **Integer** (whole numbers), **Float/Real** (decimals), **String** (text), **Boolean** (True/False). Affects operations.
*   **Initialization:** Assigning a first value to a variable (e.g., `count = 0`). Important for predictable behavior.
*   **Flowcharts:** Visual diagrams representing step-by-step logic.
    *   Key Symbols: Oval (Start/End), Rectangle (Process), Diamond (Decision), Parallelogram (Input/Output).
*   **Sanity of Data:** Checking if input data is reasonable and valid (e.g., checking if a score is within a valid range).

# Week 2: Iteration, Filtering, Selection, Pseudocode, Finding max and min, AND Operator

*   **Pseudocode:** Informal, high-level description of an algorithm. Uses plain language and programming constructs (e.g., `if`, `while`).
*   **Iteration (Loops):** Repeating a block of code.
    *   `while (condition is true) { ... }`: Loop continues as long as condition is met. Must eventually terminate.
    *   Common pattern: Processing rows in a table.
*   **Filtering/Selection (Conditionals):** Executing code based on a condition.
    *   `if (condition) { ... }`: Executes if true.
    *   `if (condition) { ... } else { ... }`: Chooses between two paths.
*   **Logical AND:** Combines conditions. (`Condition1 AND Condition2` is True ONLY if *both* are True).
*   **Finding Max/Min:** Algorithm to find the largest/smallest value by iterating through data and updating a tracking variable.

# Week 3: Multiple iterations (non-nested), Three prizes problem, Procedures, Parameters, Side effects, OR operator

*   **Procedures (Functions):** Reusable, self-contained blocks of code that perform a specific task. Improve modularity and reusability.
*   **Parameters:** Placeholders for inputs defined in a procedure's header.
*   **Arguments:** Actual values passed to parameters when a procedure is called.
*   **Side Effects:** When a procedure changes data outside its immediate scope (e.g., modifying global variables). Generally avoided for cleaner code.
*   **Multiple Iterations (Non-Nested):** Loops run one after the other. (e.g., loop A finishes, then loop B starts).
*   **Logical OR:** Combines conditions. (`Condition1 OR Condition2` is True if *at least one* is True).

# Week 4: Nested iterations, Birthday paradox, Binning

*   **Nested Iterations:** One loop (inner) completely executes for every single iteration of another loop (outer).
    *   **Purpose:** Essential for comparing all possible pairs of items (e.g., comparing every student to every other student).
    *   **Complexity:** Often involves $N \times M$ or $N^2$ operations.
*   **Birthday Paradox (Conceptual):** Illustrates that seemingly low probabilities can become high with enough items/comparisons (e.g., high chance of shared birthday in a small group).
*   **Binning:** Grouping continuous data into discrete intervals or "bins" (e.g., grouping ages into 10-year ranges).
    *   **Purpose:** Simplifies data, helps with visualization (histograms), or preprocessing for some algorithms.