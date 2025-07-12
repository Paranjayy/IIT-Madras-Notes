You got it! Let's break down the most common question patterns in Statistics I and solve a few examples for each, focusing on the straightforward steps and the logic behind them.

---

# 📚 Statistics I (BSMA1002) - Question Patterns & Example Solutions

This section summarizes the key question patterns you'll encounter in Statistics for Data Science I, providing a concise strategy and a solved example for each to illustrate the typical approach.

---

### **Pattern 1: Data Classification & Terminology**

These questions assess your foundational understanding of variable types, scales of measurement, and basic statistical vocabulary.

*   **What it's about:** Identifying if a variable is categorical or numerical, its specific measurement scale (nominal, ordinal, interval, ratio), or defining terms like population, sample, parameter, and statistic in a given scenario.
*   **How to Approach:**
    1.  **Analyze the Variable/Context:** What exactly is being measured or described?
    2.  **Categorical or Numerical?** Is it a label/category, or a number with mathematical meaning?
    3.  **If Categorical:** Can the categories be ordered? If yes, Ordinal. If no, Nominal.
    4.  **If Numerical:** Does zero mean "none"? Are ratios meaningful? If yes, Ratio. If no (zero is arbitrary), Interval.
    5.  **If Numerical (Further):** Is it obtained by counting (distinct values)? (Discrete). Or by measuring (any value in a range)? (Continuous).
    6.  **For Terminology:** What's the *whole group* of interest (Population)? The *subset studied* (Sample)? The *number from the whole* (Parameter)? The *number from the subset* (Statistic)?

---

**Example Question (Based on PYQ 76, July 2024 QDF4):**

Consider the following statements:
1.  Election symbol is a categorical variable.
2.  Election symbol has a nominal scale of measurement.
3.  Number of votes received by a candidate is a continuous variable.

Which of the following statement(s) is/are true?
(This is often a Multiple Choice Question (MCQ) or Multiple Select Question (MSQ) where you choose combinations of true statements.)

**Step-by-Step Solution:**

1.  **Analyze Statement 1:** "Election symbol is a categorical variable."
    *   **Thought Process:** An election symbol (like a 'lotus' or 'hand') is a *name* or *category*, not a number.
    *   **Conclusion:** This is **True**. It represents a quality, not a quantity.

2.  **Analyze Statement 2:** "Election symbol has a nominal scale of measurement."
    *   **Thought Process:** Since it's categorical (from Step 1), can these symbols be logically *ordered*? Is a 'lotus' greater or smaller than a 'hand'? No. When there's no inherent order, it's nominal.
    *   **Conclusion:** This is **True**. It's purely for classification.

3.  **Analyze Statement 3:** "Number of votes received by a candidate is a continuous variable."
    *   **Thought Process:** "Number of votes" means you count them (e.g., 100 votes, 101 votes). You cannot have 100.5 votes. Values that can only be whole, distinct numbers are discrete, not continuous. Continuous variables are measurements (like height or time), which can have infinite decimal places.
    *   **Conclusion:** This is **False**. It's a discrete variable.

**Final Answer:** Statements 1 and 2 are true.

---

### **Pattern 2: Summarizing & Visualizing Categorical Data**

These questions ask you to work with frequencies, proportions, or central tendencies (like the mode) for categorical data, often presented in tables or charts.

*   **What it's about:** Calculating specific counts or percentages from a frequency table or chart, or identifying the most frequent category.
*   **How to Approach:**
    1.  **Identify the Total:** Determine the grand total of all observations. This is often provided or can be calculated by summing all frequencies.
    2.  **Identify Specific Frequencies:** Find the count for the category/group of interest.
    3.  **Calculate Proportion/Percentage:** Divide the specific frequency by the relevant total. (For "proportion of X *given* Y", the denominator is the total of Y).
    4.  **For Mode:** Find the category with the highest frequency.

---

**Example Question (Based on PYQ 104, Feb 2025 QDF2):**

A table shows cuisine preferences of 150 people.
Cuisine | Frequency | Relative frequency
--- | --- | ---
Italian | 45 |
Chinese | 35 |
Mexican | ? | x
Indian | 20 |
Thai | y | 0.1
Greek | 10 |

What is the value of 'y' (frequency of Thai cuisine)?

**Step-by-Step Solution:**

1.  **Understand the Goal:** Find the frequency (count) for Thai cuisine, given its relative frequency and the total number of people.
2.  **Recall Relative Frequency Definition:** Relative Frequency = $\frac{\text{Frequency}}{\text{Total Number of Observations}}$.
3.  **Identify Known Values for Thai Cuisine:**
    *   Relative frequency (Thai) = 0.1
    *   Total Number of Observations (Total people surveyed) = 150 (given in the problem description).
    *   Frequency (Thai) = y (what we need to find).
4.  **Set up the Equation:**
    $0.1 = \frac{y}{150}$
5.  **Solve for y:**
    $y = 0.1 \times 150$
    $y = 15$

**Final Answer:** The value of y is 15.

---

### **Pattern 3: Numerical Summaries & Linear Transformations**

These questions involve calculating descriptive statistics for numerical data (mean, median, SD, etc.) or applying rules for how these statistics change when data is linearly transformed ($Y = aX + b$).

*   **What it's about:** Calculating central tendency or dispersion measures. A common variant is to see how these measures change if you add a constant, multiply by a constant, or both, to all data points.
*   **How to Approach:**
    1.  **For Basic Calculation (Mean, Median, Range, etc.):**
        *   **Order the Data:** *Crucial* for median, quartiles, and range.
        *   Apply the specific definition/formula for the required measure.
    2.  **For Linear Transformations ($Y = aX + b$):**
        *   **Identify 'a' (multiplier) and 'b' (additive constant).**
        *   **Recall the Rules for each measure:**
            *   **Mean/Median/Mode:** New = $a \times (\text{Old}) + b$. (They shift and scale).
            *   **Range/Standard Deviation/IQR:** New = $|a| \times (\text{Old})$. (They only scale, unaffected by 'b').
            *   **Variance:** New = $a^2 \times (\text{Old})$. (Scales by the square of 'a').

---

**Example Question (Based on PYQ 81, July 2024 QDF4):**

Manoj's exam marks are: 60, 70, 65, 75, 80. Nitin scored 5 marks more than Manoj in each subject. Find the mean of the marks scored by Nitin.

**Step-by-Step Solution:**

1.  **Understand the Goal:** Find Nitin's average mark. We know Manoj's marks and the relationship between Manoj's and Nitin's marks.
2.  **Analyze Manoj's Marks:**
    *   Manoj's Marks ($X$): $\{60, 70, 65, 75, 80\}$
    *   Number of subjects ($n$) = 5
3.  **Calculate Manoj's Mean ($\bar{X}$):**
    $\bar{X} = \frac{60 + 70 + 65 + 75 + 80}{5} = \frac{350}{5} = 70$.
4.  **Analyze the Transformation for Nitin's Marks:**
    *   Nitin's mark in each subject = Manoj's mark + 5.
    *   This is a linear transformation: $Y = X + 5$. Here, the multiplier $a=1$ and the additive constant $b=5$.
5.  **Apply the Rule for Mean Transformation:**
    *   If $Y = aX + b$, then the new mean $\bar{Y} = a\bar{X} + b$.
    *   So, Nitin's Mean ($\bar{Y}$) = $1 \times (\text{Manoj's Mean}) + 5$
    *   $\bar{Y} = 1 \times 70 + 5 = 70 + 5 = 75$.

**Final Answer:** The mean of Nitin's marks is 75.

---

### **Pattern 4: Association Between Variables**

These questions explore relationships between two variables, covering visual analysis (scatterplots) or numerical quantification (covariance, correlation).

*   **What it's about:** Interpreting relationships from charts (e.g., which scatterplot shows a strong negative correlation), or calculating covariance/correlation for pairs of numerical data.
*   **How to Approach:**
    1.  **For Scatterplots:**
        *   **Direction:** Does the cloud of points go up (positive), down (negative), or no clear trend?
        *   **Strength:** How tightly clustered are the points around a line? (Tight = strong; scattered = weak).
        *   **Form:** Is the trend straight (linear)?
    2.  **For Covariance:**
        *   **Calculate Means:** Find $\bar{x}$ and $\bar{y}$.
        *   **Calculate Deviations:** For each $(x,y)$ pair, find $(x - \bar{x})$ and $(y - \bar{y})$.
        *   **Multiply Deviations:** For each pair, multiply $(x - \bar{x}) \times (y - \bar{y})$.
        *   **Sum Products:** Add up all these products.
        *   **Divide by (n-1) for Sample, or N for Population.** The sign tells direction.
    3.  **For Correlation Coefficient ($r$):**
        *   **Recall:** $r = \frac{\text{Covariance}(X,Y)}{\text{SD}(X) \times \text{SD}(Y)}$.
        *   **Calculate Covariance** (as above).
        *   **Calculate Standard Deviations** for both X and Y.
        *   **Divide.** The value will be between -1 and +1. The closer to $\pm 1$, the stronger the linear relationship.

---

**Example Question (Based on PYQ 80, July 2024 QDF4):**

Find the population covariance between X and Y for the dataset:
X | -3 | -4 | -5 | 5 | 4 | 3
--- | --- | --- | --- | --- | --- | ---
Y | 10 | 5 | 3 | 3 | 5 | 10

**Step-by-Step Solution:**

1.  **Understand the Goal:** Calculate the population covariance, which measures the joint variability and direction of the linear relationship between X and Y.
2.  **List Data Points and Count (N):**
    *   $(x_i, y_i)$: $(-3, 10), (-4, 5), (-5, 3), (5, 3), (4, 5), (3, 10)$
    *   Number of pairs ($N$) = 6. (The question asks for *population* covariance, so we use $N$).
3.  **Calculate Mean of X ($\mu_X$):**
    $\mu_X = \frac{-3 + (-4) + (-5) + 5 + 4 + 3}{6} = \frac{0}{6} = 0$.
4.  **Calculate Mean of Y ($\mu_Y$):**
    $\mu_Y = \frac{10 + 5 + 3 + 3 + 5 + 10}{6} = \frac{36}{6} = 6$.
5.  **Calculate Deviations and Their Products for Each Pair:**
    We need $(x_i - \mu_X)(y_i - \mu_Y)$. Since $\mu_X = 0$, this simplifies to $x_i(y_i - \mu_Y)$.

| $x_i$ | $y_i$ | $x_i - \mu_X = x_i - 0$ | $y_i - \mu_Y = y_i - 6$ | $(x_i - \mu_X)(y_i - \mu_Y)$ |
| :---- | :---- | :-------------------- | :-------------------- | :-------------------------- |
| -3    | 10    | -3                    | $10 - 6 = 4$          | $(-3)(4) = -12$             |
| -4    | 5     | -4                    | $5 - 6 = -1$          | $(-4)(-1) = 4$              |
| -5    | 3     | -5                    | $3 - 6 = -3$          | $(-5)(-3) = 15$             |
| 5     | 3     | 5                     | $3 - 6 = -3$          | $(5)(-3) = -15$             |
| 4     | 5     | 4                     | $5 - 6 = -1$          | $(4)(-1) = -4$              |
| 3     | 10    | 3                     | $10 - 6 = 4$          | $(3)(4) = 12$               |
|       |       |                       | **Sum:**              | **$0$**                     |

6.  **Apply Covariance Formula:**
    Population Covariance ($\sigma_{XY}$) = $\frac{\sum (x_i - \mu_X)(y_i - \mu_Y)}{N}$
    $\sigma_{XY} = \frac{0}{6} = 0$.

**Final Answer:** The population covariance is 0.

---



Here's a brief summary of the key concepts and common PYQ patterns for IIT Madras Foundational Course: Statistics for Data Science I (BSMA1002).

---

# 📚 Statistics for Data Science I (BSMA1002) - Concise Summary & PYQ Patterns

This summary condenses the core concepts and recurrent question types in Statistics for Data Science I, providing a high-level overview for quick revision and pattern recognition.

---

### **Core Concepts by Week (Brief Overview)**

*   **WEEK 1: Introduction & Data Types**
    *   **Statistics Branches:** Descriptive (summarize) vs. Inferential (generalize).
    *   **Terminology:** Population (entire group) vs. Sample (subset); Parameter (population summary) vs. Statistic (sample summary); Variable (characteristic measured).
    *   **Data Types:**
        *   **Categorical (Qualitative):** Labels, non-numerical.
            *   **Nominal:** Categories with no order (e.g., gender, hair color).
            *   **Ordinal:** Categories with order, but unequal intervals (e.g., satisfaction ratings, education levels).
        *   **Numerical (Quantitative):** Measured quantities.
            *   **Interval:** Ordered, equal intervals, no true zero (e.g., temperature in Celsius).
            *   **Ratio:** Ordered, equal intervals, true zero (e.g., height, income, number of items).
        *   **Numerical Sub-types:** Discrete (countable, whole numbers) vs. Continuous (measurable, any value within range).

*   **WEEK 2: Describing Categorical Data**
    *   **Frequency Distributions:** Absolute (counts), Relative (proportions), Percentage.
    *   **Visualizations:** Bar Charts (for comparison), Pie Charts (for parts of a whole).
    *   **Central Tendency:** Mode (most frequent category) is primary; Median for Ordinal data only.

*   **WEEK 3: Describing Numerical Data**
    *   **Frequency Tables:** Grouped data into class intervals for continuous variables.
    *   **Central Tendency:**
        *   **Mean:** Average ($\frac{\sum x}{n}$). Sensitive to outliers.
        *   **Median:** Middle value when ordered. Robust to outliers.
        *   **Mode:** Most frequent value(s).
    *   **Dispersion (Spread):**
        *   **Range:** Max - Min. Highly sensitive to outliers.
        *   **Variance ($\sigma^2$/$s^2$):** Average squared deviation from mean. Units squared.
        *   **Standard Deviation ($\sigma$/$s$):** Square root of variance. Same units as data.
        *   **Quartiles ($Q_1, Q_2, Q_3$):** Divide ordered data into 4 parts. $Q_2$ is Median.
        *   **Interquartile Range (IQR):** $Q_3 - Q_1$. Robust to outliers.
    *   **Linear Transformations:** How $Y = aX + b$ affects measures ($\bar{Y}=a\bar{X}+b$, $s_Y=|a|s_X$, $s_Y^2=a^2s_X^2$, etc.).

*   **WEEK 4: Association Between Two Variables**
    *   **Two Categorical Variables:**
        *   **Contingency Tables:** Two-way tables showing joint frequencies.
        *   **Conditional Frequencies:** Crucial for assessing association (e.g., % of X given Y).
    *   **Two Numerical Variables:**
        *   **Scatterplot:** Visualizing relationship (Direction, Form, Strength, Outliers).
        *   **Covariance:** Measures direction of linear relationship (units depend on variables).
        *   **Pearson Correlation Coefficient ($r$/$\rho$):** Standardized measure of *linear* relationship strength and direction (-1 to +1).
        *   **Crucial:** Correlation $\ne$ Causation; $r=0$ means no *linear* relationship.

---

### **PYQ Patterns & Insights**

Here are the common question patterns observed in Statistics I PYQs, along with the key concepts they test and tips for solving:

1.  **Pattern 1: Data Classification & Terminology**
    *   **What it asks:** Identify the type of variable (categorical/numerical), its scale of measurement (nominal, ordinal, interval, ratio), or distinguish between population/sample/parameter/statistic.
    *   **Key Concepts Tested:** Definitions from Week 1 (Scales of Measurement, Population vs. Sample, Parameter vs. Statistic).
    *   **Tips for Solving:**
        *   **For Scales:** Ask yourself: Can I categorize it? (Nominal). Can I order it? (Ordinal). Can I subtract meaningfully? (Interval). Does it have a true zero? Can I divide meaningfully? (Ratio).
        *   **For Discrete/Continuous:** Can I count it (integers only)? (Discrete). Can I measure it with infinite precision? (Continuous).
        *   **For Pop/Sample:** Is it the *entire* group of interest (Population) or a *subset* studied (Sample)?
        *   **For Param/Stat:** Does the number describe the *population* (Parameter) or the *sample* (Statistic)?

2.  **Pattern 2: Frequency & Proportions (Categorical Data)**
    *   **What it asks:** Calculate absolute, relative, or percentage frequencies from raw data or given tables (e.g., "What proportion of X is Y?"). Interpret information presented in bar or pie charts.
    *   **Key Concepts Tested:** Frequency distributions, percentages, reading charts (Week 2).
    *   **Tips for Solving:**
        *   Always identify the **total** relevant to the question (e.g., total males vs. grand total of all people).
        *   Proportions are fractions/decimals (sum to 1); percentages are proportions $\times$ 100 (sum to 100).
        *   For charts, ensure you read labels and scales correctly.

3.  **Pattern 3: Numerical Summaries & Linear Transformations**
    *   **What it asks:** Calculate mean, median, mode, range, variance, standard deviation, quartiles, or IQR for a given numerical dataset. Crucially, it often involves understanding how these measures change after a **linear transformation** ($Y = aX + b$).
    *   **Key Concepts Tested:** Formulas for all central tendency and dispersion measures. Properties of mean, median, mode, range, variance, SD, IQR under $Y=aX+b$ transformation (Week 3).
    *   **Tips for Solving:**
        *   **Order data:** Always the first step for median, quartiles, range.
        *   **Mean/Median/Mode:** These *shift* with 'b' (addition) and *scale* with 'a' (multiplication).
        *   **Range/SD/IQR:** These are *unaffected* by 'b' (addition/subtraction) but *scale* with $|a|$ (absolute value of multiplication).
        *   **Variance:** Scales with $a^2$ (square of multiplication).
        *   Pay attention to *population* vs. *sample* variance/standard deviation formulas ($N$ vs. $n-1$).

4.  **Pattern 4: Association Between Variables**
    *   **What it asks:**
        *   For **categorical variables**: Create or interpret contingency tables, calculate conditional proportions/percentages to show association (e.g., "What percentage of X *given* Y?").
        *   For **numerical variables**: Interpret scatterplots (direction, strength, form, outliers). Calculate covariance or Pearson correlation coefficient.
    *   **Key Concepts Tested:** Contingency tables, conditional frequency (Week 4 for categorical). Scatterplots, covariance formula, Pearson correlation formula, properties of correlation (Week 4 for numerical).
    *   **Tips for Solving:**
        *   **Contingency Tables:** Read carefully whether a proportion is "of the total," "of the row total," or "of the column total."
        *   **Scatterplots:** Visually estimate if the trend is positive, negative, or none, and how tight the points are (strong/weak).
        *   **Covariance/Correlation:** Remember the interpretation of sign (+/-) for direction and magnitude for strength. The correlation coefficient is always between -1 and +1.
        *   **Crucial:** Be aware that correlation (association) does NOT imply causation.

---

This summary should provide a solid framework for understanding the types of questions you'll encounter in Statistics for Data Science I and the core knowledge needed to answer them. Good luck!

--- 
Okay, absolutely! Let's break down the general strategies for solving each type of Statistics I PYQ. Think of this as your "how-to" guide for tackling these problems, focusing on the thought process and key steps.

---

# 📈 Statistics I (BSMA1002) - Simplified Problem-Solving Guide

This guide provides a methodical approach to solving common question patterns in Statistics for Data Science I. For each pattern, we'll outline the question's goal, necessary knowledge, and a step-by-step solution strategy.

---

### **Pattern 1: Data Classification & Terminology Questions**

These questions test your fundamental understanding of what data is and how it's categorized.

*   **Goal of the Question:** To correctly identify the type of variable (e.g., categorical, numerical), its scale of measurement (nominal, ordinal, interval, ratio), or to distinguish between core statistical terms like population/sample, parameter/statistic.

*   **Key Knowledge Needed:**
    *   Definitions of **Categorical (Qualitative)** vs. **Numerical (Quantitative)** data.
    *   Definitions of **Nominal, Ordinal, Interval, Ratio** scales.
    *   Definitions of **Discrete** vs. **Continuous** numerical data.
    *   Definitions of **Population, Sample, Parameter, Statistic, Variable**.

*   **Simplified Steps to Solve:**

    1.  **Read the Variable/Context Carefully:**
        *   **What is being measured or described?** (e.g., "favorite color," "number of children," "temperature," "school performance of *all* students").

    2.  **Categorical or Numerical?**
        *   **Ask:** Is the data a label/category (like "red," "male," "good") or a number (like "10," "175 cm")?
        *   **If Labels:** It's **Categorical**. Proceed to Step 3 for scale.
        *   **If Numbers:** It's **Numerical**. Proceed to Step 4 for scale.

    3.  **If Categorical, Determine Scale (Nominal or Ordinal):**
        *   **Ask:** Can I logically order or rank these categories? (e.g., "small, medium, large" can be ordered, but "red, blue, green" cannot).
        *   **If NO order:** It's **Nominal**.
        *   **If YES order:** It's **Ordinal**.
        *   **💡 Why this step?** The type of ordering determines which descriptive measures (like median) are appropriate later.

    4.  **If Numerical, Determine Scale (Interval or Ratio):**
        *   **Ask:** Does zero (0) mean the *complete absence* of the quantity being measured? Can I meaningfully say "twice as much" or "half as much"?
        *   **If NO (zero is arbitrary, ratios not meaningful):** It's **Interval** (e.g., $0^\circ C$ temperature doesn't mean no heat; year 0 doesn't mean no time).
        *   **If YES (true zero, ratios meaningful):** It's **Ratio** (e.g., 0 height means no height; 10 kg is twice 5 kg).
        *   **💡 Why this step?** The presence of a true zero allows for multiplication/division and ratio comparisons, which are used in many advanced statistical methods.

    5.  **If Numerical, Determine Discrete or Continuous:**
        *   **Ask:** Is the data obtained by **counting** (resulting in whole, distinct numbers, like "number of students") or by **measuring** (potentially any value within a range, like "height")?
        *   **If Counting:** It's **Discrete**.
        *   **If Measuring:** It's **Continuous**.
        *   **⚠️ Important Note:** Sometimes discrete data can be large enough to be *treated* as continuous for certain analyses, but its fundamental nature remains discrete.

    6.  **For Population/Sample/Parameter/Statistic Questions:**
        *   **Identify the target group for conclusion:** This is your **Population**.
        *   **Identify the actual group data was collected from:** This is your **Sample**.
        *   **Identify the number describing the Population:** This is a **Parameter**.
        *   **Identify the number calculated from the Sample:** This is a **Statistic**.
        *   **💡 Why this step?** This distinction is critical for understanding the validity of inferences in statistics.

---

### **Pattern 2: Frequency & Proportions (Categorical Data) Questions**

These questions involve summarizing and displaying categorical data, often using tables or charts.

*   **Goal of the Question:** To calculate counts, proportions, percentages, or identify modes from categorical data, or to interpret bar/pie charts.

*   **Key Knowledge Needed:**
    *   Definitions of **Absolute, Relative, Percentage Frequency**.
    *   Understanding **Mode**.
    *   How to read **Bar Charts** and **Pie Charts**.
    *   How to use **Contingency Tables** for two categorical variables (Week 4, but often implied here).

*   **Simplified Steps to Solve:**

    1.  **Identify the Categories:**
        *   **List** all the distinct categories present in the data.

    2.  **Count Absolute Frequencies:**
        *   **Tally** how many times each category appears. This gives you the **Absolute Frequency**.
        *   **Calculate the Total Count** of all observations.

    3.  **Calculate Relative Frequencies (if needed):**
        *   For each category, **divide its absolute frequency by the total count**.
        *   **💡 Why this step?** Relative frequencies (proportions) allow for comparison across different sized datasets.

    4.  **Calculate Percentage Frequencies (if needed):**
        *   For each category, **multiply its relative frequency by 100%**.

    5.  **Identify the Mode:**
        *   **Find** the category (or categories) with the **highest absolute frequency**. This is the **Mode**.
        *   **⚠️ Important Note:** A dataset can have one mode, multiple modes, or no mode.

    6.  **For Chart Interpretation (Bar/Pie):**
        *   **Read the Title and Labels:** Understand what the axes or slices represent.
        *   **For Bar Charts:** **Compare bar heights** to see frequencies/magnitudes.
        *   **For Pie Charts:** **Look at slice sizes** to understand proportions of the whole. Sum of slices should be 100%.

    7.  **For Conditional Proportions (often in two-way tables, even if not explicitly "Week 4"):**
        *   **Identify the "given" condition:** This becomes your **denominator** (the total for that row or column).
        *   **Identify the specific count within that condition:** This is your **numerator**.
        *   **Calculate:** $\frac{\text{Numerator}}{\text{Denominator}}$.
        *   **💡 Why this step?** This tells you the likelihood of one event happening *if* another event is already known to have occurred.

---

### **Pattern 3: Numerical Summaries & Linear Transformations Questions**

These questions involve calculating or interpreting summary statistics for numerical data, especially when the data has been changed by a simple mathematical rule.

*   **Goal of the Question:** To find the mean, median, mode, range, variance, standard deviation, quartiles, or IQR for a numerical dataset. A key variation is to determine how these measures *change* after a linear transformation ($Y = aX + b$).

*   **Key Knowledge Needed:**
    *   Formulas and procedures for **Mean, Median, Mode, Range, Variance, Standard Deviation, Quartiles, IQR** (Week 3).
    *   **Properties of Measures under Linear Transformation** ($Y=aX+b$) for all these statistics (Week 3).
    *   Distinction between **Population ($N$)** and **Sample ($n-1$)** in variance/standard deviation denominators.

*   **Simplified Steps to Solve:**

    1.  **For Mean, Median, Quartiles, IQR:**
        *   **Order the Data:** **Crucial first step** for median, quartiles, and range. Arrange all numerical values from smallest to largest.
        *   **Calculate Mean:** **Sum all values and divide by the count** ($\frac{\sum x}{n}$).
        *   **Find Median:**
            *   If **odd count**, it's the **middle value**.
            *   If **even count**, it's the **average of the two middle values**.
        *   **Find Quartiles ($Q_1, Q_3$):** Find the median of the **lower half** ($Q_1$) and the **upper half** ($Q_3$) of the ordered data.
        *   **Calculate IQR:** **$Q_3 - Q_1$**.
        *   **Calculate Range:** **Maximum Value - Minimum Value**.

    2.  **For Mode:**
        *   **Identify the Most Frequent Value(s):** Look for values that repeat most often. No need to order for this.

    3.  **For Variance ($\sigma^2$ or $s^2$):**
        *   **Calculate the Mean ($\mu$ or $\bar{x}$)** first.
        *   **Calculate Deviations:** For each data point $x_i$, find $(x_i - \text{mean})$.
        *   **Square Deviations:** Square each $(x_i - \text{mean})$ value.
        *   **Sum Squared Deviations:** Add all the squared deviations.
        *   **Divide by Denominator:**
            *   For **Population Variance ($\sigma^2$): divide by $N$ (total count).**
            *   For **Sample Variance ($s^2$): divide by $n-1$ (sample count minus 1).**
        *   **⚠️ Important Note:** Pay very close attention to whether the question asks for population or sample variance/standard deviation.

    4.  **For Standard Deviation ($\sigma$ or $s$):**
        *   **Calculate the Variance** first.
        *   **Take the Square Root** of the variance.

    5.  **For Linear Transformation Questions ($Y = aX + b$):**
        *   **Identify 'a' and 'b':** Determine the multiplier ($a$) and the additive constant ($b$).
        *   **Apply the Rules (Memorize/Understand):**
            *   **Mean, Median, Mode:** New measure = $a \times (\text{Old Measure}) + b$.
            *   **Range, Standard Deviation, IQR:** New measure = $|a| \times (\text{Old Measure})$. (The additive 'b' does NOT affect spread measures).
            *   **Variance:** New Variance = $a^2 \times (\text{Old Variance})$.
        *   **💡 Why this step?** Applying these properties saves a lot of calculation time on transformed datasets.

---

### **Pattern 4: Association Between Variables Questions**

These questions explore how two variables relate to each other, using visual or numerical methods.

*   **Goal of the Question:** To identify associations between categorical variables using contingency tables, or to describe/quantify linear relationships between numerical variables using scatterplots, covariance, or correlation.

*   **Key Knowledge Needed:**
    *   **Contingency Tables:** Interpretation of joint, marginal, and conditional frequencies (Week 4).
    *   **Scatterplots:** Visual interpretation of direction, form, strength, outliers (Week 4).
    *   **Covariance:** Formula and interpretation of sign (Week 4).
    *   **Pearson Correlation Coefficient:** Formula, range, interpretation of sign and magnitude (Week 4).
    *   **Correlation $\ne$ Causation** principle.

*   **Simplified Steps to Solve:**

    1.  **For Two Categorical Variables (Contingency Tables):**
        *   **Construct/Complete the Table:** Fill in all given counts and derive missing totals (rows, columns, grand total).
        *   **Identify "Condition" and "Outcome":** If asked "Proportion of X *given* Y," then Y is the condition.
        *   **Calculate Conditional Proportion:** Divide the count in the specific cell (intersection of X and Y) by the *total of the condition* (row total or column total for Y).
        *   **💡 Why this step?** Conditional proportions are the direct way to assess if one categorical variable's distribution changes based on the other.

    2.  **For Two Numerical Variables (Scatterplot):**
        *   **Examine the Plot:**
            *   **Direction:** Do points generally go up from left to right (positive)? Down (negative)? Or no clear slope?
            *   **Form:** Do points form a relatively straight line (linear)? Or a curve (non-linear)?
            *   **Strength:** How close are the points to forming that line/curve? Are they tightly packed (strong) or widely spread (weak)?
            *   **Outliers:** Are there any points far away from the main cluster?
        *   **⚠️ Important Note:** Scatterplots are the *first* and *most important* step for numerical relationships. Don't jump straight to numbers!

    3.  **For Covariance ($s_{XY}$ or $\sigma_{XY}$):**
        *   **Calculate Means:** Find $\bar{x}$ (or $\mu_X$) and $\bar{y}$ (or $\mu_Y$).
        *   **Calculate Deviations:** For each pair $(x_i, y_i)$, find $(x_i - \bar{x})$ and $(y_i - \bar{y})$.
        *   **Calculate Products of Deviations:** Multiply the deviations for each pair: $(x_i - \bar{x})(y_i - \bar{y})$.
        *   **Sum Products:** Add up all these products.
        *   **Divide by Denominator:**
            *   For **Population Covariance ($\sigma_{XY}$): divide by $N$.**
            *   For **Sample Covariance ($s_{XY}$): divide by $n-1$.**
        *   **💡 Why this step?** The sign of covariance (positive/negative) tells you the direction of the linear relationship. The magnitude is less interpretable.

    4.  **For Pearson Correlation Coefficient ($r$ or $\rho$):**
        *   **Calculate Covariance ($s_{XY}$ or $\sigma_{XY}$)** first.
        *   **Calculate Standard Deviations:** Find $s_X$ (or $\sigma_X$) and $s_Y$ (or $\sigma_Y$).
        *   **Apply Formula:** $r = \frac{s_{XY}}{s_X s_Y}$ (or $\rho = \frac{\sigma_{XY}}{\sigma_X \sigma_Y}$).
        *   **Interpret:**
            *   **Sign:** Positive $r \implies$ positive linear relation. Negative $r \implies$ negative linear relation.
            *   **Magnitude:** Closer to $\pm 1 \implies$ stronger linear relation. Closer to $0 \implies$ weaker linear relation.
        *   **⚠️ Important Note:** Always remember correlation does NOT equal causation. A high $r$ simply means the variables move together linearly.

---

By following these simplified, step-by-step approaches, you can systematically break down any Statistics I PYQ and confidently arrive at the correct solution. Remember to always understand *why* each step is taken and what concept it relates to. Good luck with your studies!