# WEEK 1: Set Theory - Number system, Sets and their operations, Relations and functions

This week establishes the fundamental language of mathematics: sets. Understanding sets allows us to precisely define collections of objects, and from there, build concepts like relations and functions, which are critical for describing data and its transformations.

## 1.1 Number Systems

Mathematics is built upon different categories of numbers.
*   **Natural Numbers ($\mathbb{N}$):** The counting numbers. Usually includes 0 in computer science and modern set theory contexts (as specified in IITM syllabus notation).
    *   $\mathbb{N} = \{0, 1, 2, 3, \dots \}$
*   **Integers ($\mathbb{Z}$):** Whole numbers, including negative numbers and zero.
    *   $\mathbb{Z} = \{\dots, -3, -2, -1, 0, 1, 2, 3, \dots \}$
*   **Rational Numbers ($\mathbb{Q}$):** Numbers that can be expressed as a fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \ne 0$.
    *   $\mathbb{Q} = \{ \frac{p}{q} \mid p \in \mathbb{Z}, q \in \mathbb{Z}, q \ne 0 \}$
    *   Examples: $0.5 = \frac{1}{2}$, $-3 = \frac{-3}{1}$, $0.333\dots = \frac{1}{3}$.
*   **Real Numbers ($\mathbb{R}$):** All rational and irrational numbers. Irrational numbers cannot be expressed as simple fractions (e.g., $\sqrt{2}$, $\pi$, $e$). Real numbers cover the entire number line.
    *   $\mathbb{R} = \mathbb{Q} \cup \text{Irrational Numbers}$

**Relationships (Hierarchy):** $\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R}$

## 1.2 Sets and Their Operations

*   **Set:** A well-defined collection of distinct objects. Objects are called elements or members.
    *   **Notation:** Curly braces `{}`. Elements are separated by commas.
    *   **Examples:** $A = \{1, 2, 3\}$, $B = \{\text{red, blue, green}\}$.
    *   **Empty Set ($\emptyset$ or \{\}):** A set containing no elements.
    *   **Universal Set ($U$):** The set of all possible elements relevant to a particular context.
    *   **Cardinality ($|A|$):** The number of distinct elements in a set $A$.

*   **Set Operations:**
    *   **Union ($A \cup B$):** The set of all elements that are in $A$, or in $B$, or in both.
        *   $A \cup B = \{x \mid x \in A \text{ or } x \in B\}$
        *   Example: If $A=\{1,2,3\}$, $B=\{3,4,5\}$, then $A \cup B = \{1,2,3,4,5\}$.
    *   **Intersection ($A \cap B$):** The set of all elements that are common to both $A$ and $B$.
        *   $A \cap B = \{x \mid x \in A \text{ and } x \in B\}$
        *   Example: If $A=\{1,2,3\}$, $B=\{3,4,5\}$, then $A \cap B = \{3\}$.
    *   **Difference ($A - B$ or $A \setminus B$):** The set of all elements that are in $A$ but not in $B$.
        *   $A - B = \{x \mid x \in A \text{ and } x \notin B\}$
        *   Example: If $A=\{1,2,3\}$, $B=\{3,4,5\}$, then $A - B = \{1,2\}$.
    *   **Complement ($A'$ or $A^c$ or $\bar{A}$):** The set of all elements in the universal set $U$ that are not in $A$.
        *   $A' = \{x \mid x \in U \text{ and } x \notin A\}$
    *   **Subset ($A \subseteq B$):** Every element of $A$ is also an element of $B$.
        *   **Proper Subset ($A \subset B$):** $A \subseteq B$ and $A \ne B$.
    *   **Disjoint Sets:** Two sets $A$ and $B$ are disjoint if their intersection is the empty set ($A \cap B = \emptyset$).
    *   **Cartesian Product ($A \times B$):** The set of all possible ordered pairs $(a,b)$ where $a \in A$ and $b \in B$.
        *   $A \times B = \{(a,b) \mid a \in A \text{ and } b \in B\}$
        *   If $|A|=m$ and $|B|=n$, then $|A \times B| = m \times n$.
        *   Example: If $A=\{1,2\}$, $B=\{a,b\}$, then $A \times B = \{(1,a), (1,b), (2,a), (2,b)\}$.

## 1.3 Relations and Functions

*   **Relation:** A correspondence between two sets $A$ and $B$. Formally, a relation $R$ from $A$ to $B$ is any **subset of the Cartesian product $A \times B$**.
    *   If $(a,b) \in R$, we say $a$ is related to $b$ (often written as $aRb$).
    *   **Domain of R:** The set of all first elements of the ordered pairs in $R$.
    *   **Codomain of R:** The set $B$ (the set where the second elements come from).
    *   **Range of R:** The set of all second elements of the ordered pairs in $R$. (Range $\subseteq$ Codomain).

*   **Properties of Relations (on a set A, i.e., $R \subseteq A \times A$):**
    *   **Reflexive:** For every element $a \in A$, $(a,a) \in R$. (Every element is related to itself).
        *   Example: $R = \{(1,1), (2,2)\}$ on $A=\{1,2\}$.
    *   **Symmetric:** If $(a,b) \in R$, then $(b,a) \in R$. (If $a$ is related to $b$, then $b$ is related to $a$).
        *   Example: $R = \{(1,2), (2,1)\}$ on $A=\{1,2\}$.
    *   **Transitive:** If $(a,b) \in R$ and $(b,c) \in R$, then $(a,c) \in R$.
        *   Example: $R = \{(1,2), (2,3), (1,3)\}$ on $A=\{1,2,3\}$.
    *   **Equivalence Relation:** A relation that is **reflexive, symmetric, AND transitive**. (Partitions the set into disjoint equivalence classes).

*   **Function:** A special type of relation where each element in the **domain** is mapped to **exactly one** element in the **codomain**.
    *   Notation: $f: A \to B$ means $f$ is a function from set $A$ (domain) to set $B$ (codomain).
    *   **Input (argument):** An element from the domain $A$.
    *   **Output (value):** The unique element in $B$ that the input maps to, denoted $f(x)$.
    *   **Range of f:** The set of all actual output values $\{f(x) \mid x \in A\}$. (Range $\subseteq$ Codomain).

## Pattern 1.1: Cardinality of Sets and Relations

These questions often involve calculating the number of elements in a set, a Cartesian product, or an intersection of relations.

---

**Example Question (Based on PYQ 3, Feb 2025 QDF2):**
The Cartesian product $A \times A$ has 9 elements. Two of the elements of the Cartesian product are (1, 3) and (3, 7). Find the sum of all the elements in set $A$.

**Step-by-Step Solution:**

1.  **Understand Cartesian Product Cardinality:**
    *   Given $|A \times A| = 9$.
    *   We know that if $|A|=m$, then $|A \times A| = m \times m = m^2$.
    *   So, $m^2 = 9 \implies m = 3$. This means set $A$ has 3 distinct elements: $|A|=3$.

2.  **Identify Elements of A from Given Pairs:**
    *   The elements of $A \times A$ are ordered pairs $(a,b)$ where $a \in A$ and $b \in A$.
    *   We are given two elements: $(1, 3)$ and $(3, 7)$.
    *   From $(1,3)$, we know $1 \in A$ and $3 \in A$.
    *   From $(3,7)$, we know $3 \in A$ and $7 \in A$.
    *   So far, the elements identified for $A$ are $\{1, 3, 7\}$.

3.  **Confirm the Set A:**
    *   We found that $|A|=3$.
    *   The elements we identified are $\{1, 3, 7\}$, which indeed has 3 distinct elements.
    *   Therefore, $A = \{1, 3, 7\}$.

4.  **Calculate the Sum of Elements in A:**
    *   Sum $= 1 + 3 + 7 = 11$.

**Final Answer:** The sum of all elements in set A is 11.

---

## Pattern 1.2: Properties of Relations

These questions require you to determine if a given relation is reflexive, symmetric, or transitive.

---

**Example Question (Based on PYQ 60, July 2024 QDF4):**
Suppose $A = \{2, 4, 6, 8, 10, 12, 14, 16, 18, 20\}$ and $B = \{6, 12, 18\}$.
Consider the relation $R_2$ from $A$ to $B$: $R_2 = \{(a,b) \mid a \in A, b \in B, (a + b) \text{ mod } 10 = 0\}$.

Determine if $R_2$ is symmetric.

**Step-by-Step Solution:**

1.  **Recall Definition of Symmetric Relation:**
    A relation $R$ on a set $S$ is symmetric if for all $a, b \in S$, if $(a,b) \in R$, then $(b,a) \in R$.
    **Important Context:** Here, $R_2$ is a relation *from A to B*. For $(b,a)$ to be potentially in $R_2$, $b$ must be in $A$ and $a$ must be in $B$. This means the condition $(b \in A \text{ and } a \in B)$ must hold.

2.  **List some elements of $R_2$:**
    *   If $a=4 \in A, b=6 \in B$: $(4+6) \text{ mod } 10 = 10 \text{ mod } 10 = 0$. So, $(4,6) \in R_2$.
    *   If $a=14 \in A, b=6 \in B$: $(14+6) \text{ mod } 10 = 20 \text{ mod } 10 = 0$. So, $(14,6) \in R_2$.
    *   If $a=8 \in A, b=12 \in B$: $(8+12) \text{ mod } 10 = 20 \text{ mod } 10 = 0$. So, $(8,12) \in R_2$.
    (Full list from previous analysis: $R_2 = \{(4,6), (14,6), (8,12), (18,12), (2,18), (12,18)\}$)

3.  **Test for Symmetry:** Pick an element $(a,b) \in R_2$ and check if $(b,a)$ is also in $R_2$.
    *   Let's take $(4,6) \in R_2$.
    *   For $R_2$ to be symmetric, $(6,4)$ must also be in $R_2$.
    *   Check conditions for $(6,4) \in R_2$:
        *   Is $6 \in A$? Yes, $6 \in \{2, 4, \dots, 20\}$.
        *   Is $4 \in B$? No, $4 \notin \{6, 12, 18\}$.
    *   Since $4 \notin B$, the pair $(6,4)$ cannot be an element of $A \times B$, and therefore cannot be in $R_2$.

4.  **Conclusion:**
    Since we found a pair $(4,6) \in R_2$ but $(6,4) \notin R_2$, the relation $R_2$ is **not symmetric**.

**Final Answer:** $R_2$ is not symmetric.

---