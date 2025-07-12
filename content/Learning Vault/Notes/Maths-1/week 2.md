# WEEK 2: Rectangular coordinate system, Straight Lines

This week introduces the Cartesian coordinate system, which allows us to represent geometric shapes and relationships using algebraic equations. A fundamental shape is the straight line, which is extensively used in data science (e.g., linear regression).

## 2.1 Cartesian Coordinate System

*   **Definition:** A system that specifies each point uniquely in a plane by a pair of numerical coordinates, which are the signed distances to the point from two fixed perpendicular directed lines (the axes).
    *   **x-axis:** Horizontal axis.
    *   **y-axis:** Vertical axis.
    *   **Origin:** The point $(0,0)$ where axes intersect.
    *   **Ordered Pair $(x,y)$:** Represents a point's position.

## 2.2 Distance and Midpoint Formulas

*   **Distance Formula:** The distance $d$ between two points $(x_1, y_1)$ and $(x_2, y_2)$ is given by:
    $d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$
*   **Midpoint Formula:** The midpoint $M$ of a line segment connecting $(x_1, y_1)$ and $(x_2, y_2)$ is:
    $M = \left( \frac{x_1 + x_2}{2}, \frac{y_1 + y_2}{2} \right)$

## 2.3 Straight Lines

*   **Slope ($m$):** A measure of the steepness and direction of a line.
    *   **Formula:** Given two points $(x_1, y_1)$ and $(x_2, y_2)$, $m = \frac{\Delta y}{\Delta x} = \frac{y_2 - y_1}{x_2 - x_1}$ (where $x_1 \ne x_2$).
    *   **Interpretation:**
        *   $m > 0$: Line rises from left to right.
        *   $m < 0$: Line falls from left to right.
        *   $m = 0$: Horizontal line ($y = \text{constant}$).
        *   $m$ is undefined: Vertical line ($x = \text{constant}$).

*   **Equations of a Line:**
    *   **Point-Slope Form:** $y - y_1 = m(x - x_1)$. Useful when you know the slope and one point.
    *   **Slope-Intercept Form:** $y = mx + c$.
        *   $m$: slope.
        *   $c$: y-intercept (the point $(0,c)$ where the line crosses the y-axis).
    *   **Standard Form (General Form):** $Ax + By + C = 0$ (where A, B, C are constants, and A and B are not both zero).

*   **Intercepts:**
    *   **x-intercept:** The point where the line crosses the x-axis. At this point, $y=0$. To find, set $y=0$ in the equation and solve for $x$.
    *   **y-intercept:** The point where the line crosses the y-axis. At this point, $x=0$. To find, set $x=0$ in the equation and solve for $y$.

*   **Parallel and Perpendicular Lines:**
    *   **Parallel Lines:** Have the **same slope** ($m_1 = m_2$).
    *   **Perpendicular Lines:** If two non-vertical lines are perpendicular, their slopes are **negative reciprocals** ($m_1 \cdot m_2 = -1$). If one line is horizontal ($m=0$), the perpendicular line is vertical (undefined slope).

*   **Angle Between Two Lines ($\theta$):**
    *   If two lines have slopes $m_1$ and $m_2$, the acute angle $\theta$ between them is given by:
        $\tan \theta = \left| \frac{m_1 - m_2}{1 + m_1 m_2} \right|$
    *   If $1 + m_1 m_2 = 0$, the lines are perpendicular, and $\theta = 90^\circ$ or $\frac{\pi}{2}$ radians.

*   **Intersection of Lines:** To find the point where two lines intersect, solve their equations simultaneously (e.g., using substitution or elimination).

## Pattern 2.1: Line Properties and Intersections

These questions often combine finding equations of lines, determining slopes, and calculating intersection points based on given conditions (e.g., intercepts, perpendicularity).

---

**Example Question (Based on PYQ 61, July 2024 QDF4):**
Suppose $P_1(3,-2)$ and $P_2(-1, 5)$. Let $L_1$ and $L_2$ be lines passing through $P_1$ and $P_2$ respectively.
If the x-intercept of the line $L_1$ is 1 and the angle between $L_1$ and $L_2$ is $\frac{\pi}{2}$, then determine the coordinates of the point where $L_1$ and $L_2$ intersect.

**Step-by-Step Solution:**

1.  **Find the Equation of Line $L_1$:**
    *   $L_1$ passes through $P_1(3, -2)$.
    *   The x-intercept of $L_1$ is 1, meaning it also passes through the point $(1, 0)$.
    *   **Calculate the slope of $L_1$ ($m_1$):**
        $m_1 = \frac{y_2 - y_1}{x_2 - x_1} = \frac{0 - (-2)}{1 - 3} = \frac{2}{-2} = -1$.
    *   **Write the equation of $L_1$ using point-slope form ($y - y_1 = m(x - x_1)$) with point $(1,0)$ and $m_1 = -1$:**
        $y - 0 = -1(x - 1)$
        $y = -x + 1$ (Equation of $L_1$)

2.  **Find the Equation of Line $L_2$:**
    *   The angle between $L_1$ and $L_2$ is $\frac{\pi}{2}$ (or $90^\circ$). This means $L_1$ and $L_2$ are **perpendicular**.
    *   **Calculate the slope of $L_2$ ($m_2$):** Since $L_1 \perp L_2$, $m_1 \cdot m_2 = -1$.
        $(-1) \cdot m_2 = -1 \implies m_2 = 1$.
    *   $L_2$ passes through $P_2(-1, 5)$.
    *   **Write the equation of $L_2$ using point-slope form ($y - y_1 = m(x - x_1)$) with point $(-1,5)$ and $m_2 = 1$:**
        $y - 5 = 1(x - (-1))$
        $y - 5 = x + 1$
        $y = x + 6$ (Equation of $L_2$)

3.  **Find the Intersection Point of $L_1$ and $L_2$:**
    *   Solve the system of equations:
        1.  $y = -x + 1$
        2.  $y = x + 6$
    *   **Substitute Equation 1 into Equation 2 (or vice versa):**
        $-x + 1 = x + 6$
    *   **Solve for $x$:**
        $1 - 6 = x + x$
        $-5 = 2x$
        $x = -\frac{5}{2}$
    *   **Substitute $x = -\frac{5}{2}$ back into either equation (using Eq. 1):**
        $y = -(-\frac{5}{2}) + 1 = \frac{5}{2} + 1 = \frac{5}{2} + \frac{2}{2} = \frac{7}{2}$

**Final Answer:** The intersection point is $\left(-\frac{5}{2}, \frac{7}{2}\right)$.

---

## Pattern 2.2: Sum of Squared Errors (SSE) for a Line Fit

This pattern involves calculating how well a given line fits a set of data points by measuring the sum of the squared vertical distances (errors) from each point to the line.

---

**Example Question (Based on PYQ 64, July 2024 QDF4):**
Radhika has been tracking her monthly expenses and the corresponding number of outings she has with friends.
Amount spent ($y$) | 37 | 44 | 53 | 50 | 57 | 64
--- | --- | --- | --- | --- | --- | ---
Number of outings ($x$) | 5 | 7 | 9 | 8 | 10 | 12

She fitted a best-fit line to her data and obtained the equation $y = 4x + 15$. What is the value of SSE (Sum of Squared Errors) in relation to the best fit line?

**Step-by-Step Solution:**

1.  **Understand SSE (Sum of Squared Errors):**
    *   SSE measures the total squared difference between the actual observed $y$ values and the $y$ values predicted by the regression line.
    *   Formula: $\text{SSE} = \sum (y_i - \hat{y}_i)^2$, where $y_i$ is the actual amount spent, and $\hat{y}_i$ is the predicted amount spent by the line $y = 4x + 15$.

2.  **For Each Data Point, Calculate $\hat{y}$ (Predicted $y$) and $(y_i - \hat{y}_i)^2$:**
    The given line equation is $\hat{y} = 4x + 15$.

| $x_i$ (Outings) | $y_i$ (Actual Spent) | $\hat{y}_i = 4x_i + 15$ (Predicted Spent) | Error $(y_i - \hat{y}_i)$ | Squared Error $(y_i - \hat{y}_i)^2$ |
| :-------------- | :------------------- | :---------------------------------------- | :------------------------ | :---------------------------------- |
| 5               | 37                   | $4(5) + 15 = 20 + 15 = 35$                | $37 - 35 = 2$             | $2^2 = 4$                           |
| 7               | 44                   | $4(7) + 15 = 28 + 15 = 43$                | $44 - 43 = 1$             | $1^2 = 1$                           |
| 9               | 53                   | $4(9) + 15 = 36 + 15 = 51$                | $53 - 51 = 2$             | $2^2 = 4$                           |
| 8               | 50                   | $4(8) + 15 = 32 + 15 = 47$                | $50 - 47 = 3$             | $3^2 = 9$                           |
| 10              | 57                   | $4(10) + 15 = 40 + 15 = 55$               | $57 - 55 = 2$             | $2^2 = 4$                           |
| 12              | 64                   | $4(12) + 15 = 48 + 15 = 63$               | $64 - 63 = 1$             | $1^2 = 1$                           |

3.  **Sum the Squared Errors:**
    $\text{SSE} = 4 + 1 + 4 + 9 + 4 + 1 = 23$.

**Final Answer:** The value of SSE is 23.

---