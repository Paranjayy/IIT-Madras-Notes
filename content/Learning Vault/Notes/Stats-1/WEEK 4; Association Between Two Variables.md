# WEEK 4: Association Between Two Variables [[processed-syllabus#2. BSMA1002 - Statistics for Data Science I]]

This week, we move beyond describing single variables to exploring relationships between *pairs* of variables. Understanding how variables associate with each other is a core aspect of data analysis, crucial for identifying patterns and making predictions.

## 4.1 Association Between Two Categorical Variables

When you have two categorical variables, you often want to know if specific categories of one variable are more or less likely to occur with specific categories of the other.

### 4.1.1 Contingency Tables (Two-Way Tables)

*   **Definition:** A table that displays the frequency distribution of two categorical variables simultaneously. Each cell in the table represents the count of observations that fall into a specific combination of categories from both variables.
*   **Structure:**
    *   Rows represent categories of one variable.
    *   Columns represent categories of the other variable.
    *   Cells contain `joint frequencies` (counts for specific combinations).
    *   `Marginal totals` appear in the row and column margins (sum of frequencies for each category of a single variable).
    *   The `grand total` is the sum of all cell frequencies.

### Example: Contingency Table

Suppose we surveyed 100 people about their gender and their preference for coffee or tea.

|          | Coffee | Tea | Marginal Total (Gender) |
| :------- | :----- | :-- | :---------------------- |
| **Male** | 30     | 20  | 50                      |
| **Female** | 25     | 25  | 50                      |
| **Marginal Total (Drink)** | 55     | 45  | **100 (Grand Total)** |

### 4.1.2 Using Relative Frequencies in Contingency Tables

Relative frequencies (proportions or percentages) are essential for interpreting associations, as they allow for comparison regardless of the total sample size.

1.  **Joint Relative Frequencies:**
    *   **Definition:** The proportion of observations that fall into a specific combination of categories.
    *   **Calculation:** Cell frequency / Grand Total.
    *   **Example:** Proportion of males who prefer coffee = $30/100 = 0.30$ or $30\%$.

2.  **Marginal Relative Frequencies:**
    *   **Definition:** The proportion of observations for each category of a single variable (calculated using the marginal totals).
    *   **Calculation:** Marginal Total / Grand Total.
    *   **Example:** Proportion of males = $50/100 = 0.50$ or $50\%$.

3.  **Conditional Relative Frequencies:**
    *   **Definition:** The proportion of observations in a specific category of one variable, *given* that they belong to a specific category of the other variable. These are key for identifying associations.
    *   **Calculation:** Cell frequency / Relevant Row or Column Marginal Total.
    *   **Example (Condition on Gender - Row Percentage):**
        *   Proportion of Coffee drinkers *among Males* = $30/50 = 0.60$ or $60\%$.
        *   Proportion of Coffee drinkers *among Females* = $25/50 = 0.50$ or $50\%$.
    *   **Example (Condition on Drink - Column Percentage):**
        *   Proportion of Males *among Coffee drinkers* = $30/55 \approx 0.545$ or $54.5\%$.
    *   **Interpretation of Association:** If the conditional relative frequencies for a category change significantly across the conditions, it suggests an association. In our example, males ($60\%$ prefer coffee) seem more likely to prefer coffee than females ($50\%$ prefer coffee), suggesting an association between gender and drink preference. If there were *no association* (i.e., independent variables), the conditional probabilities would be roughly equal to the marginal probabilities (e.g., $P(\text{Coffee | Male}) \approx P(\text{Coffee})$).

## 4.2 Association Between Two Numerical Variables

When dealing with two numerical variables, we use different tools to describe their relationship.

### 4.2.1 Scatterplot

*   **Purpose:** The primary visual tool to display the relationship between two numerical variables. Each observation is plotted as a point on a two-dimensional graph.
*   **Characteristics to Observe:**
    1.  **Direction:**
        *   **Positive Association:** As one variable increases, the other tends to increase (points rise from left to right).
        *   **Negative Association:** As one variable increases, the other tends to decrease (points fall from left to right).
        *   **No Association:** Points are scattered randomly with no clear trend.
    2.  **Form:**
        *   **Linear:** Points tend to follow a straight line.
        *   **Non-linear:** Points follow a curve (e.g., U-shaped, exponential).
    3.  **Strength:** How closely the points cluster around the form (e.g., how tightly they cluster around a line).
        *   **Strong:** Points are very close to the form.
        *   **Weak:** Points are widely scattered.
    4.  **Outliers:** Individual points that fall outside the overall pattern of the relationship. These can heavily influence measures of association.

### 4.2.2 Covariance

*   **Definition:** A measure of the joint variability of two numerical variables. It indicates the direction of the linear relationship between them.
*   **Formulae:**
    *   **Population Covariance ($\sigma_{XY}$):** $\sigma_{XY} = \frac{\sum_{i=1}^{N} (x_i - \mu_X)(y_i - \mu_Y)}{N}$
    *   **Sample Covariance ($s_{XY}$):** $s_{XY} = \frac{\sum_{i=1}^{n} (x_i - \bar{x})(y_i - \bar{y})}{n-1}$
*   **Interpretation:**
    *   **Positive Covariance:** Indicates a positive linear relationship (as X increases, Y tends to increase).
    *   **Negative Covariance:** Indicates a negative linear relationship (as X increases, Y tends to decrease).
    *   **Near Zero Covariance:** Suggests a weak or no linear relationship.
*   **Limitations:** The magnitude of covariance depends on the units of measurement of X and Y, making it difficult to compare the strength of relationships across different datasets. For example, a covariance of 100 for height (cm) and weight (kg) is not directly comparable to a covariance of 10 for exam scores (points).

### 4.2.3 Pearson Correlation Coefficient ($r$ or $\rho$)

*   **Definition:** A standardized measure of the *linear* association between two numerical variables. It normalizes covariance, making the strength of relationship comparable across different datasets.
*   **Notation:**
    *   **Population Correlation Coefficient ($\rho$):** $\rho = \frac{\sigma_{XY}}{\sigma_X \sigma_Y}$
    *   **Sample Correlation Coefficient ($r$):** $r = \frac{s_{XY}}{s_X s_Y}$
        *   where $s_X$ and $s_Y$ are the sample standard deviations of X and Y, respectively.
*   **Interpretation:**
    *   **Range:** Always between -1 and +1, inclusive.
    *   **Sign:**
        *   Positive $r$ (closer to +1): Strong positive linear relationship.
        *   Negative $r$ (closer to -1): Strong negative linear relationship.
        *   $r$ near 0: Weak or no linear relationship.
    *   **Magnitude (Strength):**
        *   $|r| \approx 1$: Very strong linear relationship.
        *   $|r| \approx 0.7-0.9$: Strong linear relationship.
        *   $|r| \approx 0.3-0.6$: Moderate linear relationship.
        *   $|r| < 0.3$: Weak or very weak linear relationship.
    *   **Example:** An $r$ of $0.85$ indicates a strong positive linear relationship, while an $r$ of $-0.92$ indicates a very strong negative linear relationship.

### 4.2.4 Point Bi-serial Correlation Coefficient

*   **Definition:** A specific type of correlation coefficient used when one variable is numerical (interval or ratio) and the other is a binary (dichotomous) categorical variable.
*   **Binary Categorical Variable:** A categorical variable with only two possible values (e.g., Male/Female, Pass/Fail, Yes/No).
*   **Purpose:** It measures the strength and direction of the relationship between the numerical variable and the two categories of the binary variable. It's mathematically equivalent to the Pearson correlation coefficient calculated between the numerical variable and the binary variable (where the two categories are assigned arbitrary numerical values, typically 0 and 1).

## 4.3 Important Cautions about Association

*   **Correlation Does Not Imply Causation:** This is a golden rule in statistics. Just because two variables are correlated (associated) does not mean that one causes the other. There might be a third, unobserved variable (a lurking variable) influencing both, or the relationship might be coincidental.
    *   **Example:** Ice cream sales and drowning incidents are positively correlated. This does not mean ice cream causes drowning; both are related to hot weather.
*   **Linearity Assumption:** Pearson correlation coefficient measures *linear* relationships. A correlation coefficient of 0 does not mean there is no relationship at all, only that there is no *linear* relationship. There might be a strong non-linear relationship (e.g., a U-shaped pattern in a scatterplot would have a correlation close to 0 but a clear relationship).
*   **Influence of Outliers:** Outliers can heavily influence the values of covariance and Pearson correlation coefficient, potentially making a weak relationship appear strong, or vice versa. Always examine the scatterplot.

**💡 Key Takeaway:** Visualizations like scatterplots are always the first step to understand the form, direction, and strength of a relationship between numerical variables, before relying solely on numerical measures like covariance and correlation. These numerical measures quantify what the visualization shows.

---