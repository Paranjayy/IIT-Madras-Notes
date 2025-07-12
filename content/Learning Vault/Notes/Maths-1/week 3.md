# WEEK 3: Quadratic Functions

This week focuses on quadratic functions, which are characterized by a highest power of 2 for the variable. Their graphs are parabolas, and they are crucial for modeling various phenomena and in optimization problems (finding maxima/minima).

## 3.1 Definition and Graph

*   **Quadratic Function:** A function of the form $f(x) = ax^2 + bx + c$, where $a, b, c$ are constants and $a \ne 0$.
*   **Graph:** A parabola.
    *   **Direction of Opening:**
        *   If $a > 0$: Parabola opens **upwards** (has a minimum point).
        *   If $a < 0$: Parabola opens **downwards** (has a maximum point).
    *   **Vertex:** The turning point of the parabola (either the lowest point for upward opening or the highest point for downward opening).
        *   **x-coordinate of Vertex:** $x_v = -\frac{b}{2a}$
        *   **y-coordinate of Vertex:** $y_v = f(x_v) = a\left(-\frac{b}{2a}\right)^2 + b\left(-\frac{b}{2a}\right) + c$. This value is the **minimum** value of the function if $a>0$, or the **maximum** value if $a<0$.
    *   **Axis of Symmetry:** A vertical line passing through the vertex, $x = -\frac{b}{2a}$. The parabola is symmetric about this line.

## 3.2 Quadratic Equations and Roots

*   **Quadratic Equation:** An equation of the form $ax^2 + bx + c = 0$. The solutions to this equation are the **roots** (or zeros or x-intercepts) of the quadratic function $f(x) = ax^2 + bx + c$.
*   **Discriminant ($\Delta$ or $D$):** $\Delta = b^2 - 4ac$. The discriminant determines the nature of the roots:
    *   If $\Delta > 0$: Two distinct real roots.
    *   If $\Delta = 0$: Exactly one real root (a repeated root). The parabola touches the x-axis at exactly one point.
    *   If $\Delta < 0$: Two complex (non-real) roots. The parabola does not intersect the x-axis.
*   **Quadratic Formula:** The roots of $ax^2 + bx + c = 0$ are given by:
    $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$

## Pattern 3.1: Properties of Quadratic Functions

These questions test your understanding of the graph of a quadratic function (parabola), its vertex, intercepts, and the nature of its roots based on the discriminant.

---

**Example Question (Based on PYQ 66, July 2024 QDF4):**
Consider the parabola $y = x^2 + 4x + 12$. Which of the following option(s) are true? (MSQ)
**Options:**
*   The co-ordinates of vertex is (-8, 2).
*   The given equation attains it minima at x = -2. (Correct)
*   y-intercept of parabola is 12. (Correct)
*   The minimum value for the given equation is 8. (Correct)

**Step-by-Step Solution:**

The given quadratic function is $y = x^2 + 4x + 12$.
Compare with $ax^2 + bx + c$: Here, $a=1, b=4, c=12$.
Since $a=1 > 0$, the parabola opens upwards and has a **minimum** value.

1.  **Check Vertex Coordinates:**
    *   x-coordinate of vertex: $x_v = -\frac{b}{2a} = -\frac{4}{2(1)} = -2$.
    *   y-coordinate of vertex: Substitute $x_v = -2$ into the equation:
        $y_v = (-2)^2 + 4(-2) + 12 = 4 - 8 + 12 = 8$.
    *   The vertex is $(-2, 8)$.
    *   **Option 1: "The co-ordinates of vertex is (-8, 2)."** $\to$ **False**.
    *   **Option 2: "The given equation attains it minima at x = -2."** $\to$ **True**. (This is the x-coordinate of the vertex).

2.  **Check y-intercept:**
    *   The y-intercept occurs when $x=0$.
    *   $y = (0)^2 + 4(0) + 12 = 12$.
    *   The y-intercept is $(0, 12)$.
    *   **Option 3: "y-intercept of parabola is 12."** $\to$ **True**.

3.  **Check Minimum Value:**
    *   Since $a>0$, the parabola opens upwards, and the y-coordinate of the vertex is the minimum value.
    *   Minimum value = $y_v = 8$.
    *   **Option 4: "The minimum value for the given equation is 8."** $\to$ **True**.

**Final Answer:** Options 6406532780410, 6406532780411, and 6406532780412 are true.

---

## Pattern 3.2: Nature of Roots of Quadratic Equations

These questions involve using the discriminant to determine if the roots are real, distinct, repeated, or complex, and whether they are rational.

---

**Example Question (Based on PYQ 68, July 2024 QDF4):**
Consider the quadratic equation $ax^2 + bx + c = 0$ where $a, b, c$ are integers with $a \ne 0$. Which of the following option(s) are true? (MSQ)
**Options:**
*   If $b^2 - 4ac > 0$ and a perfect square then there exists a rational root of the quadratic equation.
*   If $b^2 - 4ac > 0$ and not a perfect square then there exists a rational root of the quadratic equation.
*   If $b^2 - 4ac < 0$ and a perfect square then there exists a rational root of the quadratic equation.
*   If $b^2 - 4ac < 0$ and not a perfect square then there exists a rational root of the quadratic equation.

**Step-by-Step Solution:**

The roots of a quadratic equation $ax^2 + bx + c = 0$ are given by $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$.
Let $\Delta = b^2 - 4ac$ be the discriminant.

1.  **Analyze the terms for $\Delta > 0$:**
    *   If $\Delta > 0$, then $\sqrt{\Delta}$ is a real number. This means there are two distinct real roots.
    *   **Rational Roots:** For the roots to be rational, $\sqrt{\Delta}$ must be a rational number. Since $a,b,c$ are integers, $2a$ and $-b$ are rational. For $\frac{-b \pm \sqrt{\Delta}}{2a}$ to be rational, $\sqrt{\Delta}$ must be rational. This happens if and only if $\Delta$ is a **perfect square** (of an integer or a rational number, which for integer $a,b,c$ and integer $\Delta$ means $\Delta$ is a perfect square of an integer).
    *   **Option 1: "If $b^2 - 4ac > 0$ and a perfect square then there exists a rational root..."** $\to$ **True**. (In fact, there exist *two* distinct rational roots).
    *   **Option 2: "If $b^2 - 4ac > 0$ and not a perfect square then there exists a rational root..."** $\to$ **False**. If $\Delta$ is not a perfect square (e.g., $\sqrt{2}$, $\sqrt{3}$), then $\sqrt{\Delta}$ is irrational, and thus the roots will be irrational.

2.  **Analyze the terms for $\Delta < 0$:**
    *   If $\Delta < 0$, then $\sqrt{\Delta}$ is an imaginary number (e.g., $\sqrt{-4} = 2i$).
    *   This means the roots are complex (non-real) numbers. Complex numbers are not rational.
    *   **Option 3 & 4:** Both state "If $b^2 - 4ac < 0$ ... then there exists a rational root." $\to$ **False**.

**Final Answer:** Only the first option (6406532780413) is true.

---