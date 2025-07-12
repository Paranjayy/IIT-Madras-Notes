# WEEK 1: Variables, Initialization, Iterators, Filtering, Datatypes, Flowcharts, Sanity of Data

This week lays the absolute groundwork for understanding pseudocode and computational processes. It introduces the fundamental building blocks of data and the basic flow of computation.

## 1.1 Variables and Data Types

*   **Variables:**
    *   **Definition:** A named storage location in a computer's memory that holds a value. Think of it as a labeled box where you can put different kinds of information.
    *   **Purpose:** To store data that can be used or changed during a program's execution.
    *   **Declaration:** In pseudocode, variables are often used without explicit declaration (e.g., `x = 10`), but in real programming languages, you usually declare their type first (e.g., `int x;`).
    *   **Assignment:** The act of giving a value to a variable (e.g., `x = 10`, `name = "Alice"`). The `=` sign means "assigns the value on the right to the variable on the left," not "equals."

*   **Datatypes:**
    *   **Definition:** Classifies the type of value a variable can hold. This determines what operations can be performed on it.
    *   **Common Datatypes:**
        *   **Integer (Int):** Whole numbers (e.g., 5, -100, 0).
        *   **Float/Real:** Numbers with decimal points (e.g., 3.14, -0.5, 2.0).
        *   **String:** A sequence of characters (e.g., "Hello", "IIT Madras", "123"). Enclosed in quotes.
        *   **Boolean (Bool):** Represents truth values: `True` or `False`. Used in logical conditions.
    *   **Why Datatypes Matter:**
        *   `"5" + "5"` (strings) might result in `"55"` (concatenation).
        *   `5 + 5` (integers) results in `10` (addition).
        *   Operations are type-dependent.

## 1.2 Initialization

*   **Definition:** The process of assigning an initial value to a variable when it is created or at the start of a procedure.
*   **Importance:**
    *   Ensures variables have a known state before they are used in calculations or comparisons.
    *   Prevents unpredictable behavior or errors (e.g., trying to add to an uninitialized variable).
    *   For counters, often initialized to `0`. For finding maximums, initialized to a very small number (or the first element). For finding minimums, initialized to a very large number (or the first element).

## 1.3 Iterators (Conceptual) and Filtering

*   **Iterator (Conceptual):**
    *   **Definition:** A conceptual mechanism that allows you to process items one by one from a collection (like a list or a table/dataset).
    *   **Pseudocode Representation:** Often implicitly handled by constructs like `Read the first row X from Table 1` and `Move X to Table 2` within a `while` loop that checks `Table 1 has more rows`. This effectively "iterates" through the rows.

*   **Filtering:**
    *   **Definition:** The process of selecting specific data points or items from a collection based on certain criteria or conditions.
    *   **Pseudocode Representation:** Uses `if` statements (selection) to check conditions.
    *   **Example:** `if (X.Age > 18) { ... }` - filters for individuals older than 18.

## 1.4 Flowcharts

*   **Definition:** A visual representation of a process or algorithm, showing the steps as boxes of various kinds, and their order by connecting them with arrows.
*   **Standard Symbols:**
    *   **Oval/Rounded Rectangle:** Start/End (Terminator).
    *   **Rectangle:** Process/Operation (e.g., `Calculate Total`, `Assign Value`).
    *   **Diamond:** Decision/Condition (e.g., `Is X > Y?`). Has multiple exit paths (e.g., Yes/No, True/False).
    *   **Parallelogram:** Input/Output (e.g., `Read Data`, `Print Result`).
    *   **Arrows:** Indicate the flow of control.

## 1.5 Sanity of Data

*   **Definition:** Checking data for reasonableness, consistency, and adherence to expected formats or ranges. It's about validating data quality.
*   **Importance:** "Garbage in, garbage out." Incorrect or absurd data can lead to erroneous conclusions or program crashes.
*   **Examples of Sanity Checks:**
    *   **Range Checks:** Is an age value between 0 and 120? Is a score between 0 and 100?
    *   **Type Checks:** Is a "name" variable truly a string, or is it a number?
    *   **Consistency Checks:** If "Date of Birth" is 30 November, does that make sense for a month? (A month named "November" implies 30 days, so this is valid from a day count perspective, but "30 November" directly refers to a specific date. However, an invalid date would be "31 November").
    *   **Calculated Field Checks:** Does "Total Marks" equal the sum of individual subject marks?

---

**Common PYQ Pattern: Pseudocode Debugging / Error Identification (Part 1 - Initialization & Basic Sanity)**
While Week 1 concepts are foundational, they often appear as *potential errors* in debugging questions (e.g., a variable is not initialized correctly for a max/min search, or a sanity check is missed).

**Example Question (Based on PYQ 4, July 2024 QDF4 - Data Sanity):**

The given information represents "Scores" dataset and it may have some mistakes with respect to the sanity of data. Identify all rows with such mistakes. It is a Multiple Select Question (MSQ).

| Row no. | Field        | Value        |
| :------ | :----------- | :----------- |
| Row 1   | Card number  | 1            |
| Row 2   | Name         | Harish       |
| Row 3   | Gender       | M            |
| Row 4   | Date of Birth| 30 November  |
| Row 5   | Mathematics  | 62           |
| Row 6   | Physics      | 145          |
| Row 7   | Chemistry    | 91           |
| Row 8   | Total        | 398          |

**Options:**
*   6406532780184. Row 1: Incorrect data type of card number
*   6406532780185. Row 4: Invalid Date of Birth
*   6406532780186. Row 6: Physics score is out of range (Correct)
*   6406532780187. Row 8: Total score is out of range (Correct)

**Step-by-Step Solution:**

1.  **Analyze Row 1: "Card number | 1"**
    *   **Thought Process:** A "card number" is usually an identifier. While it's a number '1', it might be represented as a string if it can have leading zeros or alphanumeric characters in other contexts. However, '1' itself as an integer is a perfectly valid data type for a card number. There's no inherent "incorrect data type" from the value '1' itself without further context (like it *must* be a string, or it *must* be unique across a larger range, etc.).
    *   **Conclusion:** No obvious mistake here without more context.

2.  **Analyze Row 4: "Date of Birth | 30 November"**
    *   **Thought Process:** The value is "30 November". Is November 30 a valid date? Yes, November has 30 days. An invalid date would be something like "31 November" or "30 February".
    *   **Conclusion:** No mistake here.

3.  **Analyze Row 6: "Physics | 145"**
    *   **Thought Process:** Marks are usually out of 100 in academic settings (implied common knowledge in such problems unless specified otherwise). A score of 145 significantly exceeds 100.
    *   **Conclusion:** This score is **out of range**. This is a mistake.

4.  **Analyze Row 8: "Total | 398"**
    *   **Thought Process:** "Total" marks should be the sum of individual subject marks (Mathematics, Physics, Chemistry).
    *   Sum of scores: $62 (\text{Maths}) + 145 (\text{Physics}) + 91 (\text{Chemistry}) = 298$.
    *   The recorded Total is 398. The calculated sum is 298. These do not match.
    *   **Conclusion:** The **Total score is out of range** (or inconsistent with other scores). This is a mistake.

**Final Answer:** Row 6 and Row 8 have mistakes.