# WEEK 1: Introduction and Type of Data, Descriptive and Inferential Statistics, Scales of Measurement

This week lays the theoretical groundwork for statistics, defining its scope, key terminology, and the crucial concept of data classification. Understanding these basics is fundamental before diving into any data analysis.

## 1.1 What is Statistics?

Statistics is the science concerned with developing and studying methods for collecting, analyzing, interpreting, and presenting empirical data. It is a vital tool for making informed decisions, drawing reliable conclusions, and understanding the world around us.

*   **Intuitive Sense:** Think of statistics as detective work for numbers. You gather clues (data), organize them, look for patterns, and then try to solve the mystery (answer questions or make predictions).

### 1.1.1 Two Main Branches of Statistics

1.  **Descriptive Statistics:**
    *   **Aim:** To summarize, organize, and describe the main features of a collection of information (data). It makes raw data understandable.
    *   **Methods:** Uses numerical summaries (like averages, percentages) and visual representations (like charts, graphs).
    *   **Example:** Calculating the average height of students in your class or creating a bar chart showing the distribution of grades. You are simply describing *what is there*.
    *   **Key Idea:** "Summarize the sample."

2.  **Inferential Statistics:**
    *   **Aim:** To draw conclusions, make predictions, or generalize from a sample of data to a larger population. It involves using probability to make statements about uncertainty.
    *   **Methods:** Hypothesis testing, confidence intervals, regression analysis.
    *   **Example:** Taking a sample of students from a university to estimate the average GPA of *all* students at that university. You are inferring something about the whole based on a part.
    *   **Key Idea:** "Generalize from sample to population."

## 1.2 Key Terminology: Population, Sample, Parameter, Statistic, Variable

Precise terminology is essential in statistics to avoid confusion.

*   **Population:**
    *   **Definition:** The entire group of individuals or objects about which information is desired. It's the complete set of all possible observations of a characteristic.
    *   **Example:** All registered voters in a country; all trees in a forest; all cars manufactured by a specific company.
    *   **Analogy:** The entire ocean you want to study.

*   **Sample:**
    *   **Definition:** A subset or a part of the population selected for study. It's often impractical or impossible to study an entire population, so we use samples.
    *   **Example:** 1000 randomly selected registered voters; 50 trees from the forest; 100 cars from a production batch.
    *   **Analogy:** A bucket of water drawn from the ocean.

*   **Parameter:**
    *   **Definition:** A numerical characteristic that describes a **population**. It's usually a fixed value, but often unknown.
    *   **Notation:** Represented by Greek letters (e.g., $\mu$ for population mean, $\sigma$ for population standard deviation).
    *   **Example:** The true average height of *all* adult males in a country.

*   **Statistic:**
    *   **Definition:** A numerical characteristic that describes a **sample**. It is calculated from sample data and is used to estimate population parameters.
    *   **Notation:** Represented by Roman letters (e.g., $\bar{x}$ for sample mean, $s$ for sample standard deviation).
    *   **Example:** The average height of 1000 randomly selected adult males from that country.
    *   **Key Relationship:** We use **statistics** from samples to make **inferences** about **parameters** of a **population**.

*   **Variable:**
    *   **Definition:** A characteristic or attribute that can be measured or observed for each unit in a population or sample. Variables are what we collect data *on*.
    *   **Example:** Age, Gender, Income, Car Brand, Number of Children.

## 1.3 Types of Data / Scales of Measurement

Classifying data is one of the most critical steps in any statistical analysis because it determines which statistical methods are appropriate. Using the wrong method can lead to incorrect conclusions.

### 1.3.1 Categorical (Qualitative) Data

*   **Definition:** Represents characteristics that are descriptive attributes or categories. They do not have inherent numerical meaning.
*   **Sub-types (Scales of Measurement for Categorical Data):**

    1.  **Nominal Scale:**
        *   **Properties:** Categories only. No inherent order or ranking. Cannot be ordered meaningfully.
        *   **Operations:** Only equality/inequality.
        *   **Examples:**
            *   **Gender:** Male, Female, Non-binary. (No inherent order).
            *   **Hair Color:** Black, Brown, Blonde, Red.
            *   **Marital Status:** Single, Married, Divorced, Widowed.
            *   **Yes/No responses:** Do you own a car? (Yes/No).

    2.  **Ordinal Scale:**
        *   **Properties:** Categories with a meaningful order or ranking. The difference between categories is not necessarily uniform or measurable.
        *   **Operations:** Equality/inequality, and order (greater than/less than).
        *   **Examples:**
            *   **Education Level:** High School, Bachelor's, Master's, PhD. (Ordered, but the "difference" between HS and Bachelor's isn't numerically comparable to Master's and PhD).
            *   **Satisfaction Rating:** Very Dissatisfied, Dissatisfied, Neutral, Satisfied, Very Satisfied.
            *   **Movie Ratings:** 1-star, 2-star, 3-star, 4-star, 5-star.
            *   **Military Rank:** Private, Corporal, Sergeant.

### 1.3.2 Numerical (Quantitative) Data

*   **Definition:** Represents characteristics that can be measured numerically. These values have a meaningful order and can be used in calculations.
*   **Sub-types (Scales of Measurement for Numerical Data):**

    1.  **Interval Scale:**
        *   **Properties:** Ordered, and the differences between values are meaningful and consistent. However, it lacks a true "zero point," meaning zero does not indicate the complete absence of the characteristic. Ratios are not meaningful.
        *   **Operations:** Equality/inequality, order, addition/subtraction.
        *   **Examples:**
            *   **Temperature in Celsius or Fahrenheit:** $0^\circ C$ does not mean "no heat." A difference between $10^\circ C$ and $20^\circ C$ is the same as $20^\circ C$ and $30^\circ C$, but $20^\circ C$ is not "twice as hot" as $10^\circ C$.
            *   **Years (e.g., historical dates):** Year 0 does not mean "no time." The difference between 1990 and 2000 is 10 years, same as 2000 and 2010.

    2.  **Ratio Scale:**
        *   **Properties:** Possesses all properties of the interval scale, PLUS it has a true, meaningful "zero point." This zero point indicates the complete absence of the characteristic being measured. Ratios are meaningful.
        *   **Operations:** Equality/inequality, order, addition/subtraction, multiplication/division.
        *   **Examples:**
            *   **Height:** 0 cm means no height. 200 cm is twice as tall as 100 cm.
            *   **Weight:** 0 kg means no weight.
            *   **Income:** 0 income means no income.
            *   **Age:** 0 years means birth.
            *   **Number of items sold:** 0 means none were sold.

### 1.3.3 Discrete vs. Continuous (Sub-classification for Numerical Data)

*   **Discrete Data:**
    *   **Definition:** Numerical data that can only take on specific, countable values (often integers). There are "gaps" between possible values.
    *   **Example:**
        *   Number of students in a class (you can't have 25.5 students).
        *   Number of cars in a parking lot.
        *   Number of heads when flipping a coin 10 times.

*   **Continuous Data:**
    *   **Definition:** Numerical data that can take on any value within a given range. There are no "gaps" between possible values. Often involve measurements.
    *   **Example:**
        *   Height of a person (can be 170 cm, 170.1 cm, 170.12 cm, etc.).
        *   Weight of an object.
        *   Time taken to complete a task.
        *   Temperature (as a measure, not just a scale).

## 1.4 Why Data Type Matters

The type of data and its scale of measurement directly influences:
*   **Appropriate Statistical Methods:** You can't calculate the mean of hair colors (nominal), but you can find the mode. You can calculate the mean of heights (ratio).
*   **Visualizations:** Bar charts for categorical, histograms for numerical, scatterplots for relationships.
*   **Interpretation of Results:** Understanding what your numbers actually mean in context.

**💡 Intuition:** Imagine trying to average "apples," "oranges," and "bananas." It doesn't make sense numerically. But you can count how many of each you have (frequency). Or, if you have small, medium, large t-shirts, you can order them (ordinal), but you can't say 'medium is twice as big as small' (not ratio). Always think about what mathematical operations are truly meaningful for your data.