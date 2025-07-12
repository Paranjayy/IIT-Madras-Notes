# Week 1: Set Theory - Number system, Sets and their operations, Relations and functions

*   **Number Systems:** Hierarchy of numbers: **Natural Numbers ($\mathbb{N}$)** (0, 1, 2...), **Integers ($\mathbb{Z}$)** (...-1, 0, 1...), **Rational Numbers ($\mathbb{Q}$)** (fractions p/q), **Real Numbers ($\mathbb{R}$)** (all rational and irrational numbers).
*   **Sets:** Well-defined collections of distinct objects.
    *   **Operations:** **Union ($\cup$)**, **Intersection ($\cap$)**, **Difference ($-$)**, **Complement ($'$)**.
    *   **Cardinality ($|A|$):** Number of elements in a set.
    *   **Cartesian Product ($A \times B$):** Set of all ordered pairs $(a,b)$.
*   **Relations:** Any subset of a Cartesian product.
    *   **Properties (on a single set A):** **Reflexive** (a,a always in R), **Symmetric** (if a,b in R then b,a in R), **Transitive** (if a,b and b,c in R then a,c in R).
    *   **Equivalence Relation:** A relation that is reflexive, symmetric, AND transitive.
*   **Functions:** Special relations where each input maps to exactly one output.

# Week 2: Rectangular coordinate system, Straight Lines

*   **Rectangular Coordinate System:** Represents points in a plane using ordered pairs $(x,y)$.
*   **Straight Lines:**
    *   **Slope ($m$):** Measure of steepness ($\frac{y_2-y_1}{x_2-x_1}$). Positive slope (up), negative slope (down), zero slope (horizontal), undefined slope (vertical).
    *   **Equations:** **Slope-Intercept form ($y=mx+c$)**, **Point-Slope form ($y-y_1=m(x-x_1)$)**.
    *   **Intercepts:** Points where line crosses x-axis (y=0) or y-axis (x=0).
    *   **Parallel Lines:** Have the **same slope** ($m_1=m_2$).
    *   **Perpendicular Lines:** Slopes are **negative reciprocals** ($m_1 \cdot m_2 = -1$).
    *   **Angle between lines:** $\tan \theta = \left| \frac{m_1 - m_2}{1 + m_1 m_2} \right|$.
    *   **Intersection:** Solve line equations simultaneously.

# Week 3: Quadratic Functions

*   **Quadratic Function:** $f(x) = ax^2 + bx + c$, where $a \ne 0$.
*   **Graph:** A **parabola**.
    *   Opens **upwards** if $a > 0$ (has a minimum).
    *   Opens **downwards** if $a < 0$ (has a maximum).
*   **Vertex:** The turning point of the parabola.
    *   **x-coordinate:** $x_v = -\frac{b}{2a}$.
    *   **y-coordinate:** $y_v = f(x_v)$, which is the minimum/maximum value of the function.
*   **Quadratic Equations:** $ax^2 + bx + c = 0$. Solutions are the **roots (zeros/x-intercepts)**.
*   **Discriminant ($\Delta = b^2 - 4ac$):** Determines the nature of the roots:
    *   $\Delta > 0$: Two distinct real roots.
    *   $\Delta = 0$: One real (repeated) root.
    *   $\Delta < 0$: Two complex (non-real) roots.
    *   **Rational Roots:** Occur when $\Delta > 0$ and $\Delta$ is a **perfect square** (and coefficients are rational).

# Week 4: Algebra of Polynomials, Graphs of Polynomials

*   **Polynomials:** Generalized functions of the form $P(x) = a_n x^n + \dots + a_0$.
    *   **Degree ($n$):** Highest exponent of $x$.
    *   **Leading Coefficient ($a_n$):** Coefficient of the highest power term.
*   **Roots (Zeros):** Values of $x$ where $P(x)=0$ (x-intercepts).
    *   **Multiplicity:** Number of times a root appears.
        *   **Even multiplicity:** Graph **touches** x-axis and turns around.
        *   **Odd multiplicity:** Graph **crosses** x-axis.
*   **Graphs of Polynomials:**
    *   **End Behavior:** Determined by the **leading term ($a_n x^n$)** as $x \to \pm \infty$. (e.g., odd degree, $a_n>0 \implies \downarrow \dots \uparrow$).
    *   **y-intercept:** $P(0) = a_0$ (the constant term).
    *   **Turning Points (Local Maxima/Minima):** Points where the graph changes direction. A polynomial of degree $n$ has at most $n-1$ turning points.