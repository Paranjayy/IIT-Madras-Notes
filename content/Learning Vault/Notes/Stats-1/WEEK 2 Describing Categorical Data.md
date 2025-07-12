# WEEK 2: Describing Categorical Data

This week, we focus on methods to summarize and visualize data that falls into distinct categories. Categorical data helps us understand frequencies, proportions, and popular choices within a dataset.

## 2.1 Describing Categorical Data

Categorical data, as discussed in Week 1, classifies observations into groups or categories. Since these categories do not have numerical meaning (beyond ordinal ranking), we describe them using counts and proportions, rather than means or standard deviations.

### 2.1.1 Frequency Distribution of Categorical Data

A frequency distribution is a fundamental way to summarize categorical data. It tells us how often each category appears in the dataset.

*   **Absolute Frequency (Count):**
    *   **Definition:** The number of times each category occurs in the dataset.
    *   **Example:** If you survey 100 people about their favorite fruit, and 40 say "Apple," then the absolute frequency for "Apple" is 40.

*   **Relative Frequency:**
    *   **Definition:** The proportion of observations that fall into a particular category. It's calculated by dividing the absolute frequency by the total number of observations.
    *   **Formula:** $\text{Relative Frequency} = \frac{\text{Absolute Frequency}}{\text{Total Number of Observations}}$
    *   **Range:** Always between 0 and 1. The sum of all relative frequencies is 1.
    *   **Example:** For "Apple" with an absolute frequency of 40 out of 100 people, the relative frequency is $\frac{40}{100} = 0.40$.

*   **Percentage Frequency:**
    *   **Definition:** The relative frequency expressed as a percentage.
    *   **Formula:** $\text{Percentage Frequency} = \text{Relative Frequency} \times 100\%$
    *   **Range:** Always between 0% and 100%. The sum of all percentage frequencies is 100%.
    *   **Example:** For "Apple", the percentage frequency is $0.40 \times 100\% = 40\%$.

### Example: Creating a Frequency Table

Suppose we have data on the preferred mode of transportation for 20 students:
(Car, Bus, Walk, Bus, Car, Walk, Bike, Car, Bus, Walk, Car, Bike, Bus, Car, Walk, Bus, Car, Bus, Walk, Bike)

1.  **List Categories:** Car, Bus, Walk, Bike
2.  **Tally Counts (Absolute Frequencies):**
    *   Car: 6
    *   Bus: 6
    *   Walk: 5
    *   Bike: 3
    *   Total: 20

3.  **Calculate Relative and Percentage Frequencies:**

| Mode of Transport | Absolute Frequency | Relative Frequency | Percentage Frequency |
| :---------------- | :----------------- | :----------------- | :------------------- |
| Car               | 6                  | $6/20 = 0.30$      | $30\%$               |
| Bus               | 6                  | $6/20 = 0.30$      | $30\%$               |
| Walk              | 5                  | $5/20 = 0.25$      | $25\%$               |
| Bike              | 3                  | $3/20 = 0.15$      | $15\%$               |
| **Total**         | **20**             | **1.00**           | **100%**             |

## 2.2 Visual Representations for Categorical Data

Visualizing data is crucial for quickly grasping patterns and insights that might not be obvious from tables alone.

*   **Bar Charts:**
    *   **Purpose:** Best for comparing the frequencies or relative frequencies of different categories. Each category is represented by a bar, and the height of the bar corresponds to its frequency.
    *   **Characteristics:**
        *   Bars are typically separated (not touching), emphasizing discrete categories.
        *   Can be vertical or horizontal.
        *   Can show absolute, relative, or percentage frequencies on the y-axis.
    *   **Example:** A bar chart showing the favorite modes of transport from the table above.

*   **Pie Charts:**
    *   **Purpose:** Ideal for illustrating parts of a whole, showing the proportion each category contributes to the total.
    *   **Characteristics:**
        *   The circle represents the total (100%).
        *   Each "slice" represents a category, with its size proportional to its frequency.
    *   **Use Cases:** Most effective when you have a small number of categories (e.g., 2-5) and want to emphasize the relative contribution of each to the whole.
    *   **Limitations:** Can become difficult to read and compare proportions with too many categories, or when categories have very similar frequencies. For precise comparisons, a bar chart is usually better.

### 2.2.1 Best Practices for Graphing Categorical Data

To ensure your visualizations are clear, accurate, and not misleading:
*   **Clear Title:** State what the graph represents.
*   **Labeled Axes:** Clearly label both axes, including units if applicable (e.g., "Frequency," "Percentage," "Mode of Transport").
*   **Meaningful Scale:** For bar charts, the y-axis should typically start at zero to avoid distorting differences between bars.
*   **Consistent Categories:** Ensure categories are distinct and non-overlapping.
*   **Appropriate Chart Type:** Choose bar charts for comparisons, pie charts for parts-of-a-whole (with few categories).
*   **Avoid 3D Effects/Clutter:** These often make charts harder to read accurately.

## 2.3 Measures of Central Tendency for Categorical Data

While numerical data uses mean and median extensively, categorical data has limited options for central tendency.

*   **Mode:**
    *   **Definition:** The category that appears most frequently in a dataset. It's the only measure of central tendency that is applicable to *all* levels of measurement (nominal, ordinal, interval, ratio).
    *   **Uniqueness:** A dataset can have one mode (unimodal), two modes (bimodal), or multiple modes (multimodal). If all categories have the same frequency, there is no mode.
    *   **Example:** In our transportation data, both "Car" and "Bus" have an absolute frequency of 6, making this dataset bimodal with modes "Car" and "Bus".
    *   **Intuition:** It represents the most common "type" or "choice".

*   **Median for Ordinal Data (and only Ordinal):**
    *   **Definition:** The middle category in an ordered dataset. It is applicable only when the categories have a meaningful order (ordinal scale).
    *   **How to find:** Order the categories, then find the category that falls at the halfway point.
    *   **Example:** For education level (High School, Bachelor's, Master's, PhD), if ordered, the median would be the category that divides the lower 50% from the upper 50%.
    *   **Why mean is not applicable:** You cannot add or average category labels (e.g., "blue" + "green" has no meaning).
    *   **Why median is not applicable for nominal:** There's no meaningful way to "order" nominal categories to find a middle point (e.g., how would you order "Male" and "Female" to find the middle?).

**💡 Insight:** The choice of statistical measure always depends on the type of data you're working with. For categorical data, frequencies and proportions are key for description, and the mode is the primary measure of central tendency.