# WEEK 3: Describing Numerical Data - Measures of Central Tendency and Dispersion

This week delves into the heart of descriptive statistics for numerical data. We will learn how to quantify the "center" of a dataset (central tendency) and how to measure its "spread" or variability (dispersion). These measures provide concise summaries that reveal much about the data's characteristics.

## 3.1 Frequency Tables for Numerical Data

While simpler for categorical data, numerical data (especially continuous) often requires grouping before creating a frequency table.

*   **Grouped Frequency Distribution:**
    *   **Purpose:** Used when numerical data has a wide range of values, making individual value frequencies impractical. Data is grouped into `class intervals` or `bins`.
    *   **Steps:**
        1.  **Determine Range:** Max value - Min value.
        2.  **Decide Number of Classes (k):** Typically 5-20 classes. No strict rule, but common guidelines exist (e.g., Sturges' formula: $k = 1 + 3.322 \log_{10} N$).
        3.  **Calculate Class Width (w):** $w \approx \frac{\text{Range}}{\text{Number of Classes}}$. Round up to a convenient number.
        4.  **Establish Class Boundaries:** Define the lower and upper limits for each class interval. Boundaries should be clear and non-overlapping.
        5.  **Tally Frequencies:** Count how many data points fall into each class.
        6.  **Calculate Midpoints (Class Marks):** The center of each class interval, often used for further calculations (e.g., for approximated mean of grouped data). Midpoint = $\frac{\text{Lower Boundary} + \text{Upper Boundary}}{2}$.
    *   **Example:** Ages of people in a town (0-10, 10-20, etc.).

## 3.2 Measures of Central Tendency (Location)

These statistics tell us about the "typical" or "middle" value in a numerical dataset.

### 3.2.1 Mean (Arithmetic Average)

*   **Definition:** The sum of all values divided by the number of values. It is the most common measure of central tendency.
*   **Notation:**
    *   **Population Mean ($\mu$):** $\mu = \frac{\sum_{i=1}^{N} x_i}{N}$ (where $N$ is population size)
    *   **Sample Mean ($\bar{x}$):** $\bar{x} = \frac{\sum_{i=1}^{n} x_i}{n}$ (where $n$ is sample size)
*   **Pros:**
    *   Uses all data values.
    *   Unique for any dataset.
    *   Foundation for many statistical tests.
*   **Cons:**
    *   **Sensitive to Outliers:** Extreme values can heavily distort the mean.
    *   Only for numerical (interval or ratio) data.
*   **Intuition:** It's the "balancing point" of the data distribution.

### 3.2.2 Median

*   **Definition:** The middle value in a dataset when the data is arranged in ascending or descending order. It divides the dataset into two equal halves.
*   **How to Find:**
    1.  **Order Data:** Arrange all data points from smallest to largest.
    2.  **Odd Number of Data Points ($n$ is odd):** The median is the value at the $\frac{n+1}{2}$-th position.
    3.  **Even Number of Data Points ($n$ is even):** The median is the average of the two middle values, at positions $\frac{n}{2}$ and $\frac{n}{2}+1$.
*   **Pros:**
    *   **Robust to Outliers:** Not affected by extreme values.
    *   Applicable to ordinal, interval, and ratio data.
*   **Cons:**
    *   Does not use all data values directly in its calculation.
*   **Intuition:** It's the "middle ground" value.

### 3.2.3 Mode

*   **Definition:** The value(s) that appear most frequently in a dataset.
*   **Uniqueness:** A dataset can have:
    *   **One mode (unimodal):** Most frequent value.
    *   **Two modes (bimodal):** Two values appear with the same highest frequency.
    *   **Multiple modes (multimodal):** More than two values with the same highest frequency.
    *   **No mode:** If all values occur with the same frequency.
*   **Pros:**
    *   Can be used for any level of measurement (nominal, ordinal, interval, ratio).
    *   Not affected by outliers.
*   **Cons:**
    *   May not be unique or may not exist.
    *   May not represent the "center" well if data is spread out.
*   **Intuition:** The most "popular" data point.

### 3.2.4 Relationship Between Mean, Median, and Mode (Skewness)

The relationship between these measures can indicate the shape of the data distribution:
*   **Symmetric Distribution (e.g., Normal Distribution):** Mean $\approx$ Median $\approx$ Mode.
*   **Right-Skewed (Positively Skewed) Distribution:** Mean > Median > Mode. The "tail" of the distribution points to the right due to high outliers pulling the mean up.
*   **Left-Skewed (Negatively Skewed) Distribution:** Mean < Median < Mode. The "tail" points to the left due to low outliers pulling the mean down.

## 3.3 Measures of Dispersion (Spread/Variability)

These statistics describe how spread out or varied the data points are.

### 3.3.1 Range

*   **Definition:** The difference between the highest (maximum) and lowest (minimum) values in a dataset.
*   **Formula:** $\text{Range} = \text{Maximum Value} - \text{Minimum Value}$
*   **Pros:** Easy to calculate and understand.
*   **Cons:**
    *   Highly sensitive to outliers (only uses two values).
    *   Doesn't tell us about the distribution of values between min and max.

### 3.3.2 Variance

*   **Definition:** The average of the squared differences from the mean. It measures how far, on average, each data point is from the mean.
*   **Why squared differences?** To ensure all differences are positive and to penalize larger deviations more heavily.
*   **Notation & Formulae:**
    *   **Population Variance ($\sigma^2$):** $\sigma^2 = \frac{\sum_{i=1}^{N} (x_i - \mu)^2}{N}$
    *   **Sample Variance ($s^2$):** $s^2 = \frac{\sum_{i=1}^{n} (x_i - \bar{x})^2}{n-1}$
        *   **Why $n-1$ for sample variance?** Using $n-1$ (degrees of freedom) instead of $n$ provides an unbiased estimate of the population variance. It's a correction factor because sample means are generally "closer" to sample data points than population means are to population data points, leading to underestimation if $n$ is used.
*   **Interpretation:** Measured in squared units of the original data. Hard to interpret directly in context (e.g., "squared dollars" for income).

### 3.3.3 Standard Deviation

*   **Definition:** The square root of the variance. It is the most widely used measure of dispersion.
*   **Notation & Formulae:**
    *   **Population Standard Deviation ($\sigma$):** $\sigma = \sqrt{\sigma^2} = \sqrt{\frac{\sum_{i=1}^{N} (x_i - \mu)^2}{N}}$
    *   **Sample Standard Deviation ($s$):** $s = \sqrt{s^2} = \sqrt{\frac{\sum_{i=1}^{n} (x_i - \bar{x})^2}{n-1}}$
*   **Pros:**
    *   Measured in the same units as the original data, making it easier to interpret than variance.
    *   Uses all data values.
    *   Less sensitive to outliers than range, but still affected.
*   **Interpretation:** A larger standard deviation means data points are, on average, farther from the mean (more spread out). A smaller standard deviation means data points are clustered closely around the mean (less spread out).
*   **Empirical Rule (68-95-99.7 Rule):** For bell-shaped (approximately normal) distributions:
    *   Approx. $68\%$ of data falls within $\pm 1$ standard deviation of the mean.
    *   Approx. $95\%$ of data falls within $\pm 2$ standard deviations of the mean.
    *   Approx. $99.7\%$ of data falls within $\pm 3$ standard deviations of the mean.

### 3.3.4 Quartiles and Percentiles

*   **Percentiles:**
    *   **Definition:** Values that divide a dataset (when ordered) into 100 equal parts. The $P$-th percentile is the value below which $P$ percent of the observations fall.
    *   **Example:** The 25th percentile is the value below which 25% of the data lies.
*   **Quartiles:**
    *   **Definition:** Special percentiles that divide an ordered dataset into four equal parts.
    *   **$Q_1$ (First Quartile):** The 25th percentile. It marks the point below which $25\%$ of the data falls. (Also known as the lower quartile).
    *   **$Q_2$ (Second Quartile):** The 50th percentile. This is the **Median**. It marks the point below which $50\%$ of the data falls.
    *   **$Q_3$ (Third Quartile):** The 75th percentile. It marks the point below which $75\%$ of the data falls. (Also known as the upper quartile).
*   **How to Calculate Quartiles (General Steps):**
    1.  Order the data from smallest to largest.
    2.  Find the Median ($Q_2$).
    3.  $Q_1$ is the median of the lower half of the data (excluding $Q_2$ if $n$ is odd).
    4.  $Q_3$ is the median of the upper half of the data (excluding $Q_2$ if $n$ is odd).
    *(Note: Various methods exist for calculating quartiles, leading to slightly different values, but the concept remains the same.)*

### 3.3.5 Interquartile Range (IQR)

*   **Definition:** The range of the middle 50% of the data. It is the difference between the third quartile ($Q_3$) and the first quartile ($Q_1$).
*   **Formula:** $\text{IQR} = Q_3 - Q_1$
*   **Pros:**
    *   **Robust to Outliers:** Since it focuses on the middle 50%, it is not affected by extreme values in the dataset.
    *   Useful for identifying the spread of the "typical" values.
*   **Use in Outlier Detection (1.5 * IQR Rule):**
    *   A data point is often considered an outlier if it falls:
        *   Below $Q_1 - (1.5 \times \text{IQR})$ (Lower Fence)
        *   Above $Q_3 + (1.5 \times \text{IQR})$ (Upper Fence)

## 3.4 Five Number Summary

*   **Definition:** A concise summary of a numerical dataset's distribution, consisting of five key values.
*   **Components:**
    1.  Minimum Value (Min)
    2.  First Quartile ($Q_1$)
    3.  Median ($Q_2$)
    4.  Third Quartile ($Q_3$)
    5.  Maximum Value (Max)
*   **Purpose:** Provides a quick overview of the data's center, spread, and potential outliers.

### 3.4.1 Box Plots (Box-and-Whisker Plots)

*   **Purpose:** A visual representation of the five-number summary. It effectively displays the distribution, skewness, and presence of outliers.
*   **Construction:**
    *   A box is drawn from $Q_1$ to $Q_3$.
    *   A line inside the box marks the median ($Q_2$).
    *   "Whiskers" extend from the box to the minimum and maximum values within the acceptable range (i.e., not outliers according to the 1.5 * IQR rule).
    *   Outliers are plotted as individual points beyond the whiskers.

**💡 Mastering these measures is fundamental.** Not only do they summarize data, but they also serve as inputs for more complex statistical analyses and machine learning models. Always choose your measures wisely based on the data type and the presence of outliers.