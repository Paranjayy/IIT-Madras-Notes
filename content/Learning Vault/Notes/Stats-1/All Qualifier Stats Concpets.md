# Week 1: Introduction and type of data, Descriptive and Inferential statistics, Scales of measurement

*   **Statistics:** Science of collecting, analyzing, interpreting data.
*   **Branches:**
    *   **Descriptive Statistics:** Summarizes, organizes, and presents data (e.g., averages, charts). "What is in our data?"
    *   **Inferential Statistics:** Draws conclusions/generalizes from a sample to a population. "What can our data tell us about the larger world?"
*   **Key Terms:**
    *   **Population:** The entire group of interest.
    *   **Sample:** A subset of the population studied.
    *   **Parameter:** A numerical characteristic of a **population** (e.g., $\mu$, $\sigma$).
    *   **Statistic:** A numerical characteristic of a **sample** (e.g., $\bar{x}$, $s$).
    *   **Variable:** A characteristic measured/observed (e.g., age, gender).
*   **Data Types / Scales of Measurement:**
    *   **Categorical (Qualitative):** Labels or categories.
        *   **Nominal:** Categories with no order (e.g., gender, hair color).
        *   **Ordinal:** Categories with a meaningful order but unequal intervals (e.g., satisfaction ratings, education levels).
    *   **Numerical (Quantitative):** Measured quantities.
        *   **Interval:** Ordered, equal intervals, **no true zero** (e.g., temperature in Celsius, years).
        *   **Ratio:** Ordered, equal intervals, **true zero** (e.g., height, weight, income, number of items).
    *   **Numerical Sub-types:** **Discrete** (countable, distinct values like counts) vs. **Continuous** (measurable, any value in range like measurements).

# Week 2: Describing categorical data

*   **Frequency Distributions:** Summarize how often categories appear.
    *   **Absolute Frequency:** Raw count for each category.
    *   **Relative Frequency:** Proportion of observations in a category ($\frac{\text{Absolute Freq}}{\text{Total}}$). Sums to 1.
    *   **Percentage Frequency:** Relative frequency $\times 100\%$. Sums to 100%.
*   **Visual Representations:**
    *   **Bar Charts:** Compare frequencies/proportions across different categories. Bars are typically separated.
    *   **Pie Charts:** Show parts of a whole, illustrating each category's proportion of the total. Best for a small number of categories.
*   **Measures of Central Tendency:**
    *   **Mode:** The category or value that appears most frequently. Applicable to all data types.
    *   **Median:** Applicable only to **ordinal data** (or higher levels) because categories must be meaningfully ordered to find a middle point.

# Week 3: Describing numerical data - Measures of central tendency and dispersion

*   **Measures of Central Tendency (Location):** Describe the "typical" or "middle" value.
    *   **Mean ($\bar{x}$ or $\mu$):** The arithmetic average. Sensitive to outliers.
    *   **Median:** The middle value when data is ordered. Robust to outliers.
    *   **Mode:** The most frequent value(s).
*   **Measures of Dispersion (Spread/Variability):** Describe how spread out the data points are.
    *   **Range:** Max Value - Min Value. Highly sensitive to outliers.
    *   **Variance ($\sigma^2$ or $s^2$):** Average of squared deviations from the mean. Units are squared.
    *   **Standard Deviation ($\sigma$ or $s$):** Square root of variance. Same units as original data; more interpretable.
    *   **Percentiles:** Values that divide ordered data into 100 equal parts.
    *   **Quartiles ($Q_1, Q_2, Q_3$):** Divide ordered data into four equal parts ($Q_2$ is the Median).
    *   **Interquartile Range (IQR):** $Q_3 - Q_1$. Represents the spread of the middle 50% of the data. Robust to outliers.
*   **Linear Transformations ($Y = aX + b$):** How operations affect measures.
    *   **Mean, Median, Mode:** New = $a \times (\text{Old}) + b$.
    *   **Range, Standard Deviation, IQR:** New = $|a| \times (\text{Old})$ (unaffected by $b$).
    *   **Variance:** New = $a^2 \times (\text{Old})$ (unaffected by $b$).

# Week 4: Association between two variables (categorical and numerical)

*   **Association between Two Categorical Variables:**
    *   **Contingency Tables (Two-Way Tables):** Display frequencies for combinations of two categorical variables.
    *   **Conditional Frequencies:** Proportion of one category given another (e.g., P(Coffee | Male) = $\frac{\text{Males who prefer Coffee}}{\text{Total Males}}$). Crucial for assessing association.
*   **Association between Two Numerical Variables:**
    *   **Scatterplot:** Visualizes relationship (each point is $(x,y)$ pair). Look for **Direction** (positive, negative, no trend), **Form** (linear, non-linear), **Strength** (strong, weak), **Outliers**.
    *   **Covariance ($s_{XY}$ or $\sigma_{XY}$):** Measures direction of linear relationship. Positive (both increase), Negative (one increases, other decreases), Zero (no linear trend). Magnitude is unit-dependent.
    *   **Pearson Correlation Coefficient ($r$ or $\rho$):** Standardized measure of **strength and direction of LINEAR relationship**. Ranges from -1 to +1.
        *   $r = +1$: Perfect positive linear.
        *   $r = -1$: Perfect negative linear.
        *   $r = 0$: No linear relationship (may have non-linear).
    *   **CRUCIAL PRINCIPLE: Correlation does NOT imply causation.**