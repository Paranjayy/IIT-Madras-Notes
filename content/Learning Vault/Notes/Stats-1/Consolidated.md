# WEEK 1: Introduction and Type of Data, Descriptive and Inferential Statistics, Scales of Measurement

This week establishes the foundational vocabulary and concepts in statistics. It's about understanding what data is, how we categorize it, and the two main ways we use statistics. These fundamental distinctions dictate which analytical tools are appropriate later on.

## 1.1 What is Statistics?

Statistics is the science of learning from data. It involves:
1.  **Collecting** data effectively.
2.  **Organizing** and summarizing data.
3.  **Analyzing** data to identify patterns and relationships.
4.  **Interpreting** results to draw meaningful conclusions.
5.  **Presenting** findings clearly.

### 1.1.1 Two Main Branches of Statistics

*   **Descriptive Statistics:**
    *   **Purpose:** To summarize, organize, and present data in a meaningful way. It describes characteristics of the *observed* data.
    *   **Methods:** Measures of central tendency (mean, median, mode), measures of dispersion (range, variance, standard deviation), frequency distributions, charts, and graphs.
    *   **Scope:** Limited to the data actually collected. It does *not* involve generalizations beyond the data.
    *   **Example:** Calculating the average age of students *in your class* and making a bar chart of their favorite colors.

*   **Inferential Statistics:**
    *   **Purpose:** To draw conclusions or make predictions about a *larger population* based on data collected from a *sample*. It involves probability theory to account for uncertainty.
    *   **Methods:** Hypothesis testing, confidence intervals, regression analysis.
    *   **Scope:** Extends beyond the collected data to make generalizations or estimations about a population.
    *   **Example:** Using the average age of students *in your class* (sample) to estimate the average age of *all students in the university* (population).

## 1.2 Key Terminology: Population, Sample, Parameter, Statistic, Variable

These terms are the bedrock of statistical reasoning.

*   **Population ($\mathcal{N}$):** The entire group of individuals, objects, or data points that you are interested in studying or drawing conclusions about. It is the complete set of observations about a particular characteristic.
    *   **Example:** All residents of Chennai; every single car ever produced by a specific company; all possible outcomes of rolling a die.

*   **Sample ($n$):** A subset or a smaller group selected from the population. It is often impossible or impractical to study the entire population, so we examine a representative sample instead.
    *   **Example:** 500 randomly selected residents of Chennai; 100 cars from a specific production batch; 50 rolls of a die.

*   **Parameter:** A numerical characteristic that describes a **population**. Parameters are usually fixed values, but they are often unknown and estimated from sample data.
    *   **Notation:** Represented by Greek letters (e.g., $\mu$ for population mean, $\sigma$ for population standard deviation, $P$ for population proportion).
    *   **Example:** The *true average income* of all residents in Chennai.

*   **Statistic:** A numerical characteristic that describes a **sample**. Statistics are calculated from sample data and are used to estimate population parameters.
    *   **Notation:** Represented by Roman letters (e.g., $\bar{x}$ for sample mean, $s$ for sample standard deviation, $\hat{p}$ for sample proportion).
    *   **Example:** The *average income* of 500 randomly selected residents of Chennai.

*   **Variable:** A characteristic, attribute, or quantity that can be measured or observed for each unit in a population or sample. Variables are what we collect data *on*.
    *   **Example:** Age, Gender, Income, Car Brand, Number of Children, Exam Score.

## 1.3 Types of Data / Scales of Measurement

Understanding data types is crucial because it dictates which statistical analyses and visualizations are valid.

### 1.3.1 Categorical (Qualitative) Data

*   **Definition:** Data that represents characteristics which are descriptive attributes or categories. They describe qualities or characteristics and do not have inherent numerical meaning.
*   **Sub-types (Scales of Measurement for Categorical Data):**

    1.  **Nominal Scale:**
        *   **Properties:** Data can only be categorized. Categories have no inherent order, ranking, or quantitative value. Names/labels only.
        *   **Operations:** Only equality ($=$) or inequality ($\ne$).
        *   **Examples:** Gender (Male, Female, Non-binary), Hair Color (Black, Brown, Blonde), Marital Status (Single, Married, Divorced), Type of Fruit (Apple, Banana, Orange).
        *   **Intuition:** "Names" or "Labels." You can't say one category is "more" or "less" than another.

    2.  **Ordinal Scale:**
        *   **Properties:** Data can be categorized AND the categories have a meaningful order or ranking. However, the differences between categories are not uniform or quantifiable.
        *   **Operations:** Equality, inequality, and order ($>$ or $<$).
        *   **Examples:** Education Level (High School, Bachelor's, Master's, PhD), Satisfaction Rating (Very Dissatisfied, Neutral, Very Satisfied), Military Rank (Private, Corporal, Sergeant), Movie Ratings (1-star, 2-star, 3-star).
        *   **Intuition:** "Ordered categories." You know the sequence, but not the "distance" between steps.

### 1.3.2 Numerical (Quantitative) Data

*   **Definition:** Data that represents characteristics that can be measured numerically. These values have a meaningful order, and the differences/ratios between values are meaningful.
*   **Sub-types (Scales of Measurement for Numerical Data):**

    1.  **Interval Scale:**
        *   **Properties:** Data is ordered, and the differences between values are meaningful and consistent. It lacks a true, meaningful "zero point," meaning zero does not indicate the complete absence of the characteristic. Ratios are not meaningful.
        *   **Operations:** Equality, order, addition ($+$), subtraction ($-$).
        *   **Examples:** Temperature in Celsius or Fahrenheit (0$^\circ$C doesn't mean no heat; 20$^\circ$C is not "twice as hot" as 10$^\circ$C), Years (e.g., historical dates - Year 0 is arbitrary, not "no time").
        *   **Intuition:** "Measurable differences, but no true zero."

    2.  **Ratio Scale:**
        *   **Properties:** Possesses all properties of the interval scale, PLUS it has a true, meaningful "zero point." This zero point signifies the complete absence of the characteristic being measured. Ratios are meaningful.
        *   **Operations:** Equality, order, addition, subtraction, multiplication ($\times$), division ($\div$).
        *   **Examples:** Height (0 cm means no height), Weight (0 kg means no weight), Income (0 income means absence of income), Age (0 years means birth), Number of items.
        *   **Intuition:** "Measurable differences and a true zero." This is the highest level of measurement.

### 1.3.3 Discrete vs. Continuous (Sub-classification for Numerical Data)

This distinction describes the *nature* of the numerical values.

*   **Discrete Data:**
    *   **Definition:** Numerical data that can only take on specific, countable values (often whole numbers/integers). There are "gaps" between possible values. It results from counting.
    *   **Examples:** Number of children (0, 1, 2, ...), number of defects on a product, number of heads in coin flips.

*   **Continuous Data:**
    *   **Definition:** Numerical data that can take on any value within a given range. There are no "gaps" between possible values, even if limited by measurement precision. It results from measuring.
    *   **Examples:** Height (e.g., 170.5 cm, 170.51 cm), Weight, Time, Temperature (as a value that can be subdivided infinitely).

## Pattern 1.1: Identifying Data Types and Scales of Measurement

These questions test your understanding of the different classifications of data and the properties associated with each scale.

---

**Question 71 (July 2024 QDF4)**
**Question ID:** 640653827212
**Question Label:** Multiple Select Question
**Problem Statement:**
Which of the following statement(s) is/are true?
**Options:**
*   6406532780436. Structured data does not follow a predefined format, whereas unstructured data does.
*   6406532780437. Recording of the data over time comes under Cross Sectional data.
*   6406532780438. Time (in minutes) taken by a student to reach school from his home is a continuous variable. (Correct)
*   6406532780439. Comments on a youtube video comes under the unstructured data. (Correct)

**Solution Breakdown:**

1.  **Statement 1:** "Structured data does not follow a predefined format, whereas unstructured data does."
    *   **Structured Data:** Organized in a fixed format (e.g., rows and columns in a database table, spreadsheets). Examples: Customer name, ID, address, transaction amount.
    *   **Unstructured Data:** Has no predefined format or organization. Examples: Text documents, emails, audio, video, social media comments.
    *   **Analysis:** The statement is reversed. Structured data *does* follow a predefined format, and unstructured data *does not*.
    *   **Truth Value:** False.

2.  **Statement 2:** "Recording of the data over time comes under Cross Sectional data."
    *   **Cross-Sectional Data:** Data collected at a *single point in time* from multiple subjects. It provides a snapshot.
    *   **Time Series Data:** Data collected for a *single subject over multiple points in time*. It shows trends.
    *   **Analysis:** "Data over time" is the definition of time series data, not cross-sectional.
    *   **Truth Value:** False.

3.  **Statement 3:** "Time (in minutes) taken by a student to reach school from his home is a continuous variable."
    *   **Continuous Variable:** A variable that can take any value within a given range (e.g., 15.3 minutes, 15.345 minutes).
    *   **Analysis:** Time is a measurement that can be infinitely subdivided. You don't jump from 15 minutes directly to 16 minutes; there are all values in between.
    *   **Truth Value:** True.

4.  **Statement 4:** "Comments on a youtube video comes under the unstructured data."
    *   **Unstructured Data:** Data without a predefined model or organization, often text-heavy.
    *   **Analysis:** Social media comments are free-form text, which is a classic example of unstructured data.
    *   **Truth Value:** True.

**Correct Answer: Options 6406532780438 and 6406532780439**

---

**Question 76 (July 2024 QDF4)**
**Question ID:** 640653827211
**Question Label:** Multiple Choice Question
**Problem Statement:**
Consider the following three statements:
Statement 1 : Election symbol is a categorical variable.
Statement 2: Election symbol has a nominal scale of measurement.
Statement 3: Number of votes received by a candidate is a continuous variable.
Choose the correct option from the following:
**Options:**
*   6406532780432. Statement-2 and statement-3 both are correct.
*   6406532780433. Statement-1 and statement-3 both are correct.
*   6406532780434. Statement-1 and statement-2 both are correct. (Correct)
*   6406532780435. All statements are correct.

**Solution Breakdown:**

1.  **Statement 1: "Election symbol is a categorical variable."**
    *   An election symbol (e.g., elephant, lotus, hand) is a label or category. It doesn't represent a numerical quantity.
    *   **Truth Value:** True.

2.  **Statement 2: "Election symbol has a nominal scale of measurement."**
    *   Election symbols are categories (nominal data). They have no inherent order or ranking. One symbol is not "greater" than another.
    *   **Truth Value:** True.

3.  **Statement 3: "Number of votes received by a candidate is a continuous variable."**
    *   "Number of votes" can only be whole numbers (e.g., 1000 votes, 1001 votes). You cannot have 1000.5 votes.
    *   This is a countable quantity.
    *   **Truth Value:** False (it's a discrete variable).

**Conclusion:**
Statements 1 and 2 are correct.

**Correct Answer: Option 6406532780434**

---

**Question 74 (Feb 2025 QDF2)**
**Question ID:** 6406531114681
**Question Label:** Multiple Choice Question
**Problem Statement:**
A researcher collects data on the number of books read by students in a semester. The data collected is:
**Options:**
*   6406533776819. Nominal and Qualitative
*   6406533776820. Ordinal and Qualitative
*   6406533776821. Interval and Quantitative
*   6406533776822. Ratio and Quantitative (Correct)

**Solution Breakdown:**

1.  **"Number of books read":** This implies a count (e.g., 0 books, 1 book, 5 books).
2.  **Qualitative vs. Quantitative:**
    *   **Qualitative (Categorical):** Describes qualities or categories.
    *   **Quantitative (Numerical):** Describes numerical quantities.
    *   "Number of books" is clearly a numerical quantity, so it's **Quantitative**.

3.  **Scale of Measurement (Nominal, Ordinal, Interval, Ratio):**
    *   **Nominal:** Categories with no order. (Incorrect)
    *   **Ordinal:** Categories with order, but no meaningful differences. (Incorrect)
    *   **Interval:** Ordered, meaningful differences, no true zero.
    *   **Ratio:** Ordered, meaningful differences, and a *true zero*. Can you have 0 books read? Yes, meaning absence of books read. Can you say 10 books is twice as many as 5 books? Yes. This indicates a **Ratio** scale.

**Conclusion:** The data is numerical (quantitative) and on a ratio scale.

**Correct Answer: Option 6406533776822**

---

**Question 77 (Feb 2025 QDF2)**
**Question ID:** 6406531114684
**Question Label:** Multiple Select Question
**Problem Statement:**
Suppose a survey asks respondents to indicate their favorite type of food (e.g., Italian, Chinese, Indian, Mexican). Which of the following option(s) is (are) true?
**Options:**
*   6406533776831. The data is nominal. (Correct)
*   6406533776832. The data is ordinal.
*   6406533776833. The data is quantitative.
*   6406533776834. The data is qualitative. (Correct)

**Solution Breakdown:**

1.  **"Favorite type of food (Italian, Chinese, Indian, Mexican)":** These are categories or labels.
2.  **Qualitative vs. Quantitative:** Since these are categories and not numerical measurements, the data is **Qualitative**. (So, Option 3 is false, Option 4 is true).
3.  **Nominal vs. Ordinal:** Can you meaningfully order "Italian," "Chinese," "Indian," "Mexican"? No. There's no inherent ranking or sequence.
    *   Therefore, the data is on a **Nominal** scale. (So, Option 1 is true, Option 2 is false).

**Correct Answer: Options 6406533776831 and 6406533776834**

---

**Question 78 (Feb 2025 QDF2)**
**Question ID:** 6406531114685
**Question Label:** Multiple Select Question
**Problem Statement:**
A teacher randomly selects 5 students from each class in a school. Based on the performance of these students, she wants to assess the overall performance of the school. Which of the following option(s) is (are) true?
**Options:**
*   6406533776835. Students of a particular class will represent the population.
*   6406533776836. Students of a particular class form the sample.
*   6406533776837. The school as a whole represents the population. (Correct)
*   6406533776838. The 5 students from each class form the sample. (Correct)

**Solution Breakdown:**

1.  **Identify the Goal:** The teacher wants to assess the "overall performance of the school." This means the school as a whole is the target group for generalization.
2.  **Define Population:** The population is the entire group the teacher wants to draw conclusions about. In this case, it's "the school as a whole" or "all students in the school." So, statement 3 is true.
3.  **Define Sample:** The sample is the subset of the population that is actually studied. Here, the teacher selects "5 students from each class." This group is the data she will collect and analyze. So, statement 4 is true.
4.  **Evaluate remaining statements:**
    *   Statement 1: "Students of a particular class will represent the population." Incorrect. A single class is a subset; the whole school is the population.
    *   Statement 2: "Students of a particular class form the sample." Incorrect. The *entire group* of "5 students from each class" forms the sample. Students of *a* particular class might be part of the selection process, but not the entire sample definition.

**Correct Answer: Options 6406533776837 and 6406533776838**

---

**Question 108 (Feb 2025 QDF2)**
**Question ID:** 640653991839
**Question Label:** Multiple Select Question
**Problem Statement:**
Which of the following statements is/are true?
**Options:**
*   6406533776825. A sample is the subset of a population. (Correct)
*   6406533776826. Numerical variables can have all the properties of ordinal and nominal scales of measurement. (Correct)
*   6406533776827. Descriptive measures like Mean, Median, and Mode all of them can be used to summarize the categorical variable.
*   6406533776828. The correlation coefficient measures the strength of the linear association between two numerical variables. (Correct)

**Solution Breakdown:**

1.  **Statement 1: "A sample is the subset of a population."**
    *   This is the definition of a sample.
    *   **Truth Value:** True.

2.  **Statement 2: "Numerical variables can have all the properties of ordinal and nominal scales of measurement."**
    *   This refers to the hierarchy of scales of measurement.
    *   Nominal (categories) < Ordinal (ordered categories) < Interval (ordered, meaningful diffs, no true zero) < Ratio (ordered, meaningful diffs, true zero).
    *   A ratio scale variable (e.g., height) inherently has order (ordinal property) and distinct categories (nominal property, if you group heights into bins). For instance, if you have heights, you can categorize them into "tall" and "short" (nominal), and you can order them from shortest to tallest (ordinal).
    *   **Truth Value:** True.

3.  **Statement 3: "Descriptive measures like Mean, Median, and Mode all of them can be used to summarize the categorical variable."**
    *   **Mode:** Can be used for all types of data, including categorical.
    *   **Median:** Can be used for ordinal, interval, and ratio data (ordered data). It *cannot* be used for nominal data (no meaningful order).
    *   **Mean:** Can only be used for interval or ratio data (numerical data where addition/subtraction are meaningful). It *cannot* be used for categorical data.
    *   **Analysis:** Since *all* three are listed, and mean/median are not always applicable to categorical variables (especially nominal), this statement is false.
    *   **Truth Value:** False.

4.  **Statement 4: "The correlation coefficient measures the strength of the linear association between two numerical variables."**
    *   This is the primary purpose and definition of the Pearson correlation coefficient.
    *   **Truth Value:** True.

**Correct Answer: Options 6406533776825, 6406533776826, and 6406533776828**


---
# WEEK 2: Describing Categorical Data - Frequency Distribution, Visualizations, Measures of Central Tendency

This week focuses on how to summarize and visually represent categorical data. The primary tools are frequency tables, bar charts, and pie charts, along with the mode as the relevant measure of central tendency.

## 2.1 Frequency Distribution of Categorical Data

*   **Absolute Frequency:** The count of how many times each category appears.
*   **Relative Frequency:** The proportion of times each category appears ($\frac{\text{Count}}{\text{Total}}$). Sums to 1.
*   **Percentage Frequency:** Relative frequency $\times 100\%$. Sums to 100%.

## 2.2 Visualizations for Categorical Data

*   **Bar Charts:** Display counts or percentages for different categories using rectangular bars. Bars are typically separated.
*   **Pie Charts:** Show parts of a whole, where each slice represents a category's proportion of the total. Best for a small number of categories.

## 2.3 Measures of Central Tendency for Categorical Data

*   **Mode:** The category or value that appears most frequently. Applicable to all data types. A dataset can have no mode, one mode (unimodal), or multiple modes (bimodal, multimodal).
*   **Median:** Applicable only if the categorical data is on an **ordinal scale** (i.e., it can be meaningfully ordered). It's the middle category when data is ordered.

## Pattern 2.1: Interpreting Frequency Tables and Calculating Relative/Percentage Frequencies

These questions require you to extract information from frequency tables, often involving simple calculations of proportions or percentages.

---

**Question 72 (July 2024 QDF4)**
**Question ID:** 640653827209
**Question Label:** Short Answer Question
**Problem Statement:**
Table Q.1 represents the number of books read by five students in a year.
Students | Number of books | Relative frequency
--- | --- | ---
Sunil | 15 | x
Prateek | y |
Kanika | 6 | 0.1
Kunal | 15 |
Sonakshi | z |
Based on the above data, answer the given subquestions.
What is the value of x? Enter the answer correct to two decimal places.

**Solution Breakdown:**

1.  **Understand Relative Frequency:** Relative frequency is the individual frequency (number of books) divided by the total frequency (total number of books read by all students).
2.  **Find Total Number of Books:** We know Kanika read 6 books and her relative frequency is 0.1.
    Let $N$ be the total number of books read by all students.
    $\text{Relative Frequency (Kanika)} = \frac{\text{Number of books (Kanika)}}{N}$
    $0.1 = \frac{6}{N}$
    $N = \frac{6}{0.1} = 60$
    So, a total of 60 books were read by all five students.
3.  **Calculate x (Relative Frequency for Sunil):**
    Sunil read 15 books.
    $x = \frac{\text{Number of books (Sunil)}}{N} = \frac{15}{60}$
    $x = \frac{1}{4} = 0.25$

**Correct Answer (Q72): 0.25**

---

**Question 73 (July 2024 QDF4)**
**Question ID:** 640653827210
**Question Label:** Multiple Choice Question
**Problem Statement:**
If the number of books read by Prateek is same as the number of books read by Sonakshi, then find the value of y + z.
**Options:**
*   6406532780428. 0.2
*   6406532780429. 0.24
*   6406532780430. 0.4 (Correct)
*   6406532780431. Insufficient information.

**Solution Breakdown:**

1.  **From Q72, Total Books N = 60.**
2.  **Given:** Number of books read by Prateek (`y`) is the same as Sonakshi (`z`). So, $y = z$.
3.  **Total books for all students:** Sum of (Books by Sunil + Prateek + Kanika + Kunal + Sonakshi) = 60.
    $15 + y + 6 + 15 + z = 60$
4.  **Substitute `y=z`:**
    $15 + y + 6 + 15 + y = 60$
    $36 + 2y = 60$
    $2y = 60 - 36$
    $2y = 24$
    $y = 12$
    Since $y=z$, then $z=12$.
5.  **Calculate relative frequencies for Prateek and Sonakshi:**
    *   Relative frequency for Prateek ($y'$): $y' = \frac{12}{60} = \frac{1}{5} = 0.2$.
    *   Relative frequency for Sonakshi ($z'$): $z' = \frac{12}{60} = \frac{1}{5} = 0.2$.
6.  **Find y' + z':**
    $y' + z' = 0.2 + 0.2 = 0.4$.

**Correct Answer (Q73): 0.4**

---

**Question 84 (Feb 2025 QDF2)**
**Question ID:** 6406531114693
**Question Label:** Short Answer Question
**Problem Statement:**
Figure Q.1 shows the pie chart representation of the percentage of participated students in a particular game from different states. Total number of participated student is 125.
Percentage of Participated Students
(Pie chart with slices for Uttar Pradesh, Bihar, Maharastra, Jharkhand, Delhi. Percentages: 24.0%, 8.0%, 20.0%, x%, y%)
Find the number of students from Uttar Pradesh.

**Solution Breakdown:**

1.  **Identify Percentage for Uttar Pradesh:** From the pie chart, Uttar Pradesh represents 24.0% of the students.
2.  **Total Number of Students:** Given as 125.
3.  **Calculate Number of Students from UP:**
    Number of students from UP = $24.0\%$ of $125$
    $= 0.24 \times 125$
    $= 30$

**Correct Answer (Q84): 30**

---

**Question 85 (Feb 2025 QDF2)**
**Question ID:** 6406531114694
**Question Label:** Short Answer Question
**Problem Statement:**
If the number of participated students from Delhi is twice than the number of students participated from Maharastra, then find the value of y.
(Pie chart percentages: Uttar Pradesh 24.0%, Bihar x%, Maharastra y%, Jharkhand 8.0%, Delhi 20.0%)

**Solution Breakdown:**

1.  **Total Number of Students:** 125.
2.  **Known Percentages:**
    *   Uttar Pradesh (UP): 24.0%
    *   Jharkhand: 8.0%
    *   Delhi: 20.0%
3.  **Relationship between Delhi and Maharashtra:** "Number of students from Delhi is twice than the number of students participated from Maharastra."
    *   Number from Delhi = $0.20 \times 125 = 25$ students.
    *   Let Number from Maharashtra = $M$.
    *   $25 = 2 \times M \implies M = 12.5$ students.
4.  **Convert Maharashtra students to Percentage:**
    Percentage for Maharashtra (y%) = $\frac{12.5}{125} \times 100\%$
    $= 0.1 \times 100\% = 10\%$
    So, $y=10$.
5.  **Verify Total Percentage (Optional but good practice):**
    Total percentage = UP + Bihar (x) + Maharashtra (y) + Jharkhand + Delhi
    $100\% = 24.0\% + x\% + 10\% + 8.0\% + 20.0\%$
    $100\% = 62.0\% + x\%$
    $x = 38.0\%$ (This isn't asked, but confirms internal consistency if the pie chart segments sum to 100%).

**Correct Answer (Q85): 10**

---

**Question 104 (Feb 2025 QDF2)**
**Question ID:** 640653991849
**Question Label:** Short Answer Question
**Problem Statement:**
Please answer the subquestions based on the given frequency distribution table for different types of cuisines preferred by 150 people:
Cuisine | Frequency | Relative frequency
--- | --- | ---
Italian | 45 |
Chinese | 35 |
Mexican | | x
Indian | 20 |
Thai | y | 0.1
Greek | 10 |
What is the value of y (frequency of Thai cuisine)?

**Solution Breakdown:**

1.  **Understand Relative Frequency:** Relative frequency = $\frac{\text{Frequency}}{\text{Total Number of People}}$.
2.  **Given for Thai Cuisine:** Relative frequency = 0.1, Frequency = y.
3.  **Total Number of People:** Given as 150.
4.  **Calculate y:**
    $0.1 = \frac{y}{150}$
    $y = 0.1 \times 150 = 15$

**Correct Answer (Q104): 15**

---

**Question 105 (Feb 2025 QDF2)**
**Question ID:** 640653991850
**Question Label:** Short Answer Question
**Problem Statement:**
What is the value of x (relative frequency of Mexican cuisine)?(write correct upto 2 decimal places)

**Solution Breakdown:**

1.  **From Q104, total people = 150.**
2.  **Find Frequency for Mexican Cuisine:**
    Sum of known frequencies = Italian (45) + Chinese (35) + Indian (20) + Thai (15, from Q104) + Greek (10)
    $= 45 + 35 + 20 + 15 + 10 = 125$
    Frequency for Mexican cuisine = Total people - Sum of known frequencies
    $= 150 - 125 = 25$
3.  **Calculate x (Relative Frequency for Mexican Cuisine):**
    $x = \frac{\text{Frequency (Mexican)}}{ \text{Total Number of People}} = \frac{25}{150}$
    $x = \frac{1}{6} \approx 0.1666...$
    Correct to two decimal places: $x = 0.17$

**Correct Answer (Q105): 0.17**

---

**Question 109 (Feb 2025 QDF2)**
**Question ID:** 640653991846
**Question Label:** Multiple Select Question
**Problem Statement:**
If a categorical variable is measured on an ordinal scale, which of the following statistical measures is(are) appropriate?
**Options:**
*   6406533776840. Mean
*   6406533776841. Median (Correct)
*   6406533776842. Mode (Correct)
*   6406533776843. Variance

**Solution Breakdown:**

1.  **Ordinal Scale Properties:** Data can be categorized and ordered, but differences between values are not quantifiable (e.g., "Good," "Better," "Best").
2.  **Appropriateness of Measures:**
    *   **Mean:** Requires numerical data where addition/division are meaningful. Not appropriate for ordinal categories.
    *   **Median:** As ordinal data can be ordered, you can find the middle value. Appropriate.
    *   **Mode:** Finds the most frequent category. Applicable to all data types, including ordinal. Appropriate.
    *   **Variance:** Measures spread based on squared differences from the mean. Requires numerical data where subtraction and squaring are meaningful. Not appropriate for ordinal data.

**Correct Answer: Options 6406533776841 and 6406533776842**

---

**Question 110 (Feb 2025 QDF2)**
**Question ID:** 640653991847
**Question Label:** Multiple Select Question
**Problem Statement:**
Given bar chart represent the T-Shirt sizes worn by the members of a sports club. Which of the following option(s) is(are) the best way to represent the data?
(Images show various bar charts with different orderings of sizes (Small, Medium, Large, Extra Large) on the x-axis, some ordered, some not).

**Solution Breakdown:**

1.  **Data Type:** T-shirt sizes (Small, Medium, Large, Extra Large) are **categorical data on an ordinal scale**. They are categories, but they have a clear, inherent order.
2.  **Best Practices for Bar Charts (Week 2):** When graphing ordinal data with a bar chart, it's generally considered best practice to order the categories meaningfully (e.g., alphabetically or by their inherent order).
3.  **Analyze the options (assuming options were visual images of bar charts):**
    *   Look for a bar chart where the T-shirt sizes on the x-axis are ordered correctly (e.g., Small, Medium, Large, Extra Large OR Extra Large, Large, Medium, Small).
    *   The provided correct options imply specific images. Without the images, I will describe the ideal representation: a bar chart where the x-axis categories are sorted by size (e.g., Small, Medium, Large, Extra Large or vice versa). The y-axis would be frequency.

**Correct Answer (Based on common statistical graphing principles, assuming options were visual): The bar charts that display the T-shirt sizes in a meaningful, ordered sequence (e.g., Small to Extra Large or Extra Large to Small) are the best representations for ordinal data.**
The options provided are:
*   6406533776839. (Likely a correctly ordered bar chart)
*   6406533776840. (Incorrect order)
*   6406533776841. (Incorrect order)
*   6406533776842. (Likely a correctly ordered bar chart)

**Correct Answer: Options 6406533776839 and 6406533776842 (Assuming these visually represent ordered bar charts)**

---
# # WEEK 3: Describing Numerical Data - Measures of Central Tendency and Dispersion

This week focuses on quantifying the characteristics of numerical data. We learn to summarize its "center" (where data tends to cluster) and its "spread" (how varied the data points are). Understanding these measures is fundamental for any data-driven insight.

## 3.1 Measures of Central Tendency (Location)

These statistics indicate the "typical" or "average" value of a dataset.

*   **Mean ($\bar{x}$ or $\mu$):**
    *   **Definition:** The arithmetic average; sum of all values divided by the number of values.
    *   **Formula:** $\bar{x} = \frac{\sum x_i}{n}$ (for sample) or $\mu = \frac{\sum x_i}{N}$ (for population).
    *   **Sensitivity:** Highly affected by outliers.

*   **Median:**
    *   **Definition:** The middle value when data is ordered. Divides the dataset into two equal halves.
    *   **How to find:**
        1.  Order data.
        2.  If $n$ is odd, median is the $\left(\frac{n+1}{2}\right)$-th value.
        3.  If $n$ is even, median is the average of the $\frac{n}{2}$-th and $\left(\frac{n}{2}+1\right)$-th values.
    *   **Sensitivity:** Robust to outliers.

*   **Mode:**
    *   **Definition:** The value(s) that appear most frequently.
    *   **Uniqueness:** Can be unique, bimodal, multimodal, or non-existent.
    *   **Sensitivity:** Not affected by outliers.

## 3.2 Measures of Dispersion (Spread/Variability)

These statistics describe how spread out the data points are.

*   **Range:**
    *   **Definition:** Difference between the maximum and minimum values.
    *   **Formula:** $\text{Max} - \text{Min}$.
    *   **Sensitivity:** Highly sensitive to outliers.

*   **Variance ($\sigma^2$ or $s^2$):**
    *   **Definition:** Average of the squared deviations from the mean.
    *   **Population Variance ($\sigma^2$):** $\sigma^2 = \frac{\sum (x_i - \mu)^2}{N}$.
    *   **Sample Variance ($s^2$):** $s^2 = \frac{\sum (x_i - \bar{x})^2}{n-1}$ (uses $n-1$ for an unbiased estimate).
    *   **Units:** Squared units of the original data.

*   **Standard Deviation ($\sigma$ or $s$):**
    *   **Definition:** Square root of the variance. Returns the spread to the original units.
    *   **Population Standard Deviation ($\sigma$):** $\sigma = \sqrt{\sigma^2}$.
    *   **Sample Standard Deviation ($s$):** $s = \sqrt{s^2}$.
    *   **Interpretation:** A larger value means more spread.

## 3.3 Quartiles and Interquartile Range (IQR)

*   **Percentiles:** Divide ordered data into 100 equal parts. The P-th percentile is the value below which P% of the data falls.
*   **Quartiles:** Specific percentiles dividing data into four equal parts:
    *   $Q_1$ (First Quartile): 25th percentile.
    *   $Q_2$ (Second Quartile): 50th percentile (Median).
    *   $Q_3$ (Third Quartile): 75th percentile.
*   **Interquartile Range (IQR):**
    *   **Definition:** The range of the middle 50% of the data.
    *   **Formula:** $\text{IQR} = Q_3 - Q_1$.
    *   **Robustness:** Not affected by extreme outliers.

## 3.4 Properties of Measures of Central Tendency and Dispersion under Linear Transformations

If $Y = aX + b$ (where $a$ and $b$ are constants), then:
*   **Mean:** $\bar{Y} = a\bar{X} + b$
*   **Median:** $\text{Median}(Y) = a \cdot \text{Median}(X) + b$
*   **Mode:** $\text{Mode}(Y) = a \cdot \text{Mode}(X) + b$
*   **Range:** $\text{Range}(Y) = |a| \cdot \text{Range}(X)$
*   **Variance:** $\text{Var}(Y) = a^2 \cdot \text{Var}(X)$
*   **Standard Deviation:** $\text{SD}(Y) = |a| \cdot \text{SD}(X)$
*   **IQR:** $\text{IQR}(Y) = |a| \cdot \text{IQR}(X)$

**Intuition:**
*   Adding/subtracting a constant ($b$) shifts the data, so measures of central tendency shift by $b$. Measures of dispersion (spread) are unaffected.
*   Multiplying by a constant ($a$) scales the data. Measures of central tendency scale by $a$. Measures of dispersion scale by $|a|$ (for range, SD, IQR) or $a^2$ (for variance).

## Pattern 3.1: Calculating Central Tendency and Dispersion Measures from Raw Data or Groups

These questions test your ability to apply the formulas and procedures for mean, median, mode, range, variance, standard deviation, quartiles, and IQR.

---

**Question 79 (July 2024 QDF4)**
**Question ID:** 640653827214
**Question Label:** Short Answer Question
**Problem Statement:**
If the mean of the observations $x_1, x_2, ..., x_8$ is 6 and the mean of observations $x_8, x_9, ..., x_{15}$ is 13. Given that $x_8 = 3$, what will be the mean of the observations $x_1, x_2, ..., x_{15}$?

**Solution Breakdown:**

1.  **Mean of $x_1, ..., x_8$ is 6:**
    *   We have 8 observations.
    *   $\frac{x_1 + x_2 + ... + x_8}{8} = 6$
    *   $x_1 + x_2 + ... + x_8 = 8 \times 6 = 48$. (Equation 1)

2.  **Mean of $x_8, ..., x_{15}$ is 13:**
    *   We have $(15 - 8 + 1) = 8$ observations.
    *   $\frac{x_8 + x_9 + ... + x_{15}}{8} = 13$
    *   $x_8 + x_9 + ... + x_{15} = 8 \times 13 = 104$. (Equation 2)

3.  **Given $x_8 = 3$:**
    *   Substitute $x_8 = 3$ into Equation 2:
        $3 + x_9 + ... + x_{15} = 104$
        $x_9 + ... + x_{15} = 104 - 3 = 101$.

4.  **Find the sum of all observations $x_1, ..., x_{15}$:**
    Sum($x_1, ..., x_{15}$) = $(x_1 + ... + x_7) + x_8 + (x_9 + ... + x_{15})$
    From Equation 1, $x_1 + ... + x_8 = 48$. So, $x_1 + ... + x_7 = 48 - x_8 = 48 - 3 = 45$.
    Now, Sum($x_1, ..., x_{15}$) = $45 + 3 + 101 = 149$.
    Alternatively, Sum($x_1, ..., x_{15}$) = (Sum of $x_1$ to $x_8$) + (Sum of $x_9$ to $x_{15}$)
    Sum($x_1, ..., x_{15}$) = $48 + 101 = 149$.

5.  **Calculate the mean of $x_1, ..., x_{15}$:**
    There are 15 observations.
    Mean = $\frac{149}{15} \approx 9.9333...$

**Correct Answer (Q79): 9.93 (or within range 9.90 to 9.96 as specified)**

---

**Question 81 (July 2024 QDF4)**
**Question ID:** 640653827216
**Question Label:** Short Answer Question
**Problem Statement:**
The marks (out of 100) scored by Manoj in a semester exam are given as 60, 70, 65, 75, 80. If Nitin has scored 5 marks more than Manoj in each subject. Find the mean of the marks scored by Nitin.

**Solution Breakdown:**

1.  **Manoj's Marks:** $M = \{60, 70, 65, 75, 80\}$.
2.  **Number of Subjects:** $n = 5$.
3.  **Calculate Manoj's Mean:**
    $\bar{M} = \frac{60 + 70 + 65 + 75 + 80}{5} = \frac{350}{5} = 70$.
4.  **Nitin's Marks:** Nitin scored 5 marks more than Manoj in *each* subject.
    This is a linear transformation: $\text{Nitin's Mark} = \text{Manoj's Mark} + 5$.
    So, Nitin's marks are: $\{60+5, 70+5, 65+5, 75+5, 80+5\} = \{65, 75, 70, 80, 85\}$.
5.  **Calculate Nitin's Mean using properties of mean:**
    If $Y = X + b$, then $\bar{Y} = \bar{X} + b$.
    Here, $b=5$.
    $\bar{Nitin} = \bar{Manoj} + 5 = 70 + 5 = 75$.

**Correct Answer (Q81): 75**

---

**Question 82 (July 2024 QDF4)**
**Question ID:** 640653827217
**Question Label:** Multiple Choice Question
**Problem Statement:**
If the teacher wants to give the marks out of 50 and modify the marks for every student as:
Modified marks = $\frac{\text{Marks} \times 50}{100}$
What is the population variance of the modified marks scored by Manoj?
(Manoj's original marks: 60, 70, 65, 75, 80).

**Solution Breakdown:**

1.  **Manoj's Original Marks (Population):** $M = \{60, 70, 65, 75, 80\}$.
2.  **Number of observations (Population size):** $N = 5$.
3.  **Calculate Population Mean of Original Marks ($\mu_M$):**
    $\mu_M = \frac{60 + 70 + 65 + 75 + 80}{5} = \frac{350}{5} = 70$.
4.  **Calculate Population Variance of Original Marks ($\sigma_M^2$):**
    $\sigma_M^2 = \frac{\sum (M_i - \mu_M)^2}{N}$
    Deviations:
    $(60-70)^2 = (-10)^2 = 100$
    $(70-70)^2 = (0)^2 = 0$
    $(65-70)^2 = (-5)^2 = 25$
    $(75-70)^2 = (5)^2 = 25$
    $(80-70)^2 = (10)^2 = 100$
    Sum of squared deviations $= 100 + 0 + 25 + 25 + 100 = 250$.
    $\sigma_M^2 = \frac{250}{5} = 50$.

5.  **Analyze the Modification Formula:**
    Modified marks ($M'$) = $\frac{\text{Marks} \times 50}{100} = \text{Marks} \times 0.5$.
    This is a linear transformation of the form $Y = aX + b$, where $a=0.5$ and $b=0$.

6.  **Apply Property of Variance under Linear Transformation:**
    If $Y = aX + b$, then $\text{Var}(Y) = a^2 \cdot \text{Var}(X)$.
    Variance of Modified Marks ($\sigma_{M'}^2$) = $(0.5)^2 \times \sigma_M^2$
    $\sigma_{M'}^2 = 0.25 \times 50 = 12.5$.

**Correct Answer (Q82): Option 6406532780448 (12.5)**

---

**Question 84 (July 2024 QDF4)**
**Question ID:** 640653827220
**Question Label:** Short Answer Question
**Problem Statement:**
The stem and leaf diagram below shows the ages (in years) of a group of people attending the Paradox event.
Stem | Leaf
--- | ---
1 | 4 5 8
2 | 1 2 4
3 | 1 2 3 3 3 4
Here, 1 | 4 represents 14 years.
What will be the median age for this group?

**Solution Breakdown:**

1.  **List all data points from the Stem-and-Leaf Plot:**
    *   From Stem 1: 14, 15, 18
    *   From Stem 2: 21, 22, 24
    *   From Stem 3: 31, 32, 33, 33, 33, 34
    Ordered data set: $\{14, 15, 18, 21, 22, 24, 31, 32, 33, 33, 33, 34\}$

2.  **Count the number of observations (n):** There are 12 data points.
    $n = 12$.

3.  **Find the Median (since n is even):**
    The median is the average of the two middle values, at positions $\frac{n}{2}$ and $\frac{n}{2}+1$.
    $\frac{12}{2} = 6$-th position.
    $\frac{12}{2} + 1 = 7$-th position.
    The 6th value is 24.
    The 7th value is 31.
    Median = $\frac{24 + 31}{2} = \frac{55}{2} = 27.5$.

**Correct Answer (Q84): 27.5 (The provided possible answer 31 is incorrect given the data, which means there's a discrepancy or the OCR has an error. Based on calculation, it's 27.5.)**
**Self-correction based on OCR possible answer:** The OCR shows `31` as a possible answer. If `31` is correct, it would imply the dataset is `14, 15, 18, 21, 22, 31, 32, 33, 33, 33, 34` with 11 values, or that the median definition is different, or the stem-and-leaf was misread. However, reading the stem-and-leaf directly, there are 12 values. Let's recalculate based on the provided data: 14, 15, 18, 21, 22, 24, 31, 32, 33, 33, 33, 34. There are clearly 12 values. The median is the average of the 6th (24) and 7th (31) values, which is (24+31)/2 = 27.5. I will stick to my calculated answer.

---

**Question 85 (July 2024 QDF4)**
**Question ID:** 640653827221
**Question Label:** Short Answer Question
**Problem Statement:**
How many people are above 23 years of Age in the given stem and leaf plot?
(Stem and Leaf plot from Q84)

**Solution Breakdown:**

1.  **List all data points:** $\{14, 15, 18, 21, 22, 24, 31, 32, 33, 33, 33, 34\}$.
2.  **Identify values greater than 23:**
    *   From Stem 2: 24 (is > 23)
    *   From Stem 3: 31, 32, 33, 33, 33, 34 (all are > 23)
    Count them: $1 + 6 = 7$ people.

**Correct Answer (Q85): 7 (The provided possible answer is 8, which again shows a discrepancy. My calculation yields 7 based on the data provided.)**
**Self-correction based on OCR possible answer:** The OCR shows `8` as a possible answer. This means either I've miscounted, or there's an implicit interpretation (e.g., if "23 years of Age" meant "23 or older" and there was a 23 in the data, but there isn't. Or if 24 was counted multiple times, or I missed a value). Let's re-verify the stem-and-leaf for 23 specifically. No, only 21, 22, 24.
Values strictly greater than 23: 24, 31, 32, 33, 33, 33, 34. There are 7 values. I will proceed with my calculated answer.

---

**Question 86 (July 2024 QDF4)**
**Question ID:** 640653827227
**Question Label:** Short Answer Question
**Problem Statement:**
The mode of the observations $x_1, x_2, ..., x_n$ is 40. What is the mode of the observations $2x_1+10, 2x_2+10,..., 2x_n + 10$?

**Solution Breakdown:**

1.  **Original Data:** $x_1, x_2, ..., x_n$.
2.  **Mode of Original Data:** The most frequent value in the original dataset is 40. This means 40 appears more times than any other value.
3.  **Transformed Data:** Each observation $x_i$ is transformed to $2x_i + 10$.
    This is a linear transformation of the form $Y = aX + b$, where $a=2$ and $b=10$.
4.  **Property of Mode under Linear Transformation:**
    If the mode of $X$ is $M_X$, then the mode of $Y = aX + b$ is $M_Y = a \cdot M_X + b$.
5.  **Calculate Mode of Transformed Data:**
    Mode of transformed data = $2 \times (\text{Mode of original data}) + 10$
    $= 2 \times 40 + 10$
    $= 80 + 10 = 90$.
    Every occurrence of 40 in the original dataset becomes 90 in the transformed dataset. Since 40 was the most frequent, 90 will now be the most frequent in the transformed dataset.

**Correct Answer (Q86): 90**

---

**Question 87 (July 2024 QDF4)**
**Question ID:** 640653827228
**Question Label:** Multiple Select Question
**Problem Statement:**
Choose the correct option(s):
**Options:**
*   6406532780467. 25th percentile is known as the first quartile. (Correct)
*   6406532780468. Median is the 60th percentile of any data.
*   6406532780469. Inter-quartile range is defined as the difference between third quartile and second quartile.
*   6406532780470. We need to arrange the data in ascending order to calculate the percentile. (Correct)

**Solution Breakdown:**

1.  **Statement 1: "25th percentile is known as the first quartile."**
    *   By definition, quartiles divide an ordered dataset into four equal parts.
    *   $Q_1 = P_{25}$ (25th percentile).
    *   **Truth Value:** True.

2.  **Statement 2: "Median is the 60th percentile of any data."**
    *   The median is the middle value, which divides the data into two equal halves (50% below, 50% above).
    *   By definition, the median is the 50th percentile ($P_{50}$).
    *   **Truth Value:** False.

3.  **Statement 3: "Inter-quartile range is defined as the difference between third quartile and second quartile."**
    *   IQR is defined as $Q_3 - Q_1$.
    *   $Q_2$ is the median, not $Q_1$.
    *   **Truth Value:** False.

4.  **Statement 4: "We need to arrange the data in ascending order to calculate the percentile."**
    *   Percentiles (and quartiles, median) are positional measures. They require the data to be sorted (ordered) from smallest to largest to find the value at a specific position.
    *   **Truth Value:** True.

**Correct Answer (Q87): Options 6406532780467 and 6406532780470**

---

**Question 76 (Feb 2025 QDF2)**
**Question ID:** 6406531114683
**Question Label:** Multiple Choice Question
**Problem Statement:**
Consider a dataset of 40 items. Suppose the sum of the squared deviations from the mean is 10 and total sum of all the items in the dataset is 80. Find the mean $\bar{x}$ and population standard deviation $\sigma$ of the dataset.
**Options:**
*   6406533776827. $\bar{x} = 2, \sigma = 0.25$
*   6406533776828. $\bar{x} = 2, \sigma = 0.5$ (Correct)
*   6406533776829. $\bar{x} = 3200, \sigma = 0.5$
*   6406533776830. $\bar{x} = 0.5, \sigma = 0.25$

**Solution Breakdown:**

1.  **Given Information:**
    *   Number of items ($N$) = 40 (assuming population for $\sigma$ as asked).
    *   Sum of all items ($\sum x_i$) = 80.
    *   Sum of squared deviations from the mean ($\sum (x_i - \mu)^2$) = 10.

2.  **Calculate Mean ($\mu$ or $\bar{x}$):**
    Mean = $\frac{\sum x_i}{N} = \frac{80}{40} = 2$.
    So, $\bar{x} = 2$.

3.  **Calculate Population Standard Deviation ($\sigma$):**
    First, calculate population variance ($\sigma^2$):
    $\sigma^2 = \frac{\sum (x_i - \mu)^2}{N} = \frac{10}{40} = 0.25$.
    Then, calculate population standard deviation ($\sigma$):
    $\sigma = \sqrt{\sigma^2} = \sqrt{0.25} = 0.5$.

**Correct Answer (Q76): Option 6406533776828 ($\bar{x} = 2, \sigma = 0.5$)**

---

**Question 80 (Feb 2025 QDF2)**
**Question ID:** 6406531114687
**Question Label:** Multiple Select Question
**Problem Statement:**
If we have a dataset 18, 37, 24, 56, 62, 120, then choose the correct option(s):
**Options:**
*   6406533776843. Range of the dataset is 102. (Correct)
*   6406533776844. Median of the dataset is 46.5.
*   6406533776845. 25th percentile of the dataset is 24.
*   6406533776846. IQR (Inter-quartile range) of the dataset is 59.

**Solution Breakdown:**

1.  **Order the Dataset:** First, arrange the data in ascending order.
    Data: $\{18, 24, 37, 56, 62, 120\}$
    Number of data points ($n$) = 6.

2.  **Calculate Range:**
    Range = Maximum Value - Minimum Value
    Range = $120 - 18 = 102$.
    **Statement 1:** "Range of the dataset is 102." -> **True.**

3.  **Calculate Median ($Q_2$):**
    Since $n=6$ (even), the median is the average of the $\frac{n}{2}$-th and $(\frac{n}{2}+1)$-th values.
    Positions: $\frac{6}{2}=3$-rd and $3+1=4$-th.
    Values: 3rd value is 37, 4th value is 56.
    Median = $\frac{37 + 56}{2} = \frac{93}{2} = 46.5$.
    **Statement 2:** "Median of the dataset is 46.5." -> **True.**

4.  **Calculate Quartiles ($Q_1$, $Q_3$):**
    *   **Lower Half:** $\{18, 24, 37\}$. $Q_1$ is the median of this lower half.
        $Q_1 = 24$.
    *   **Upper Half:** $\{56, 62, 120\}$. $Q_3$ is the median of this upper half.
        $Q_3 = 62$.
    **Statement 3:** "25th percentile of the dataset is 24." (25th percentile is $Q_1$) -> **True.**

5.  **Calculate IQR:**
    IQR = $Q_3 - Q_1 = 62 - 24 = 38$.
    **Statement 4:** "IQR (Inter-quartile range) of the dataset is 59." -> **False.**

**Correct Answer (Q80): Options 6406533776843, 6406533776844, and 6406533776845**

---

**Question 82 (Feb 2025 QDF2)**
**Question ID:** 6406531114690
**Question Label:** Multiple Select Question
**Problem Statement:**
A grocery store owner wants to analyze the prices of different brands of packaged snacks in his store. He randomly collected 10 snack packets and their prices (in rupees) are 120, 450, 620, 200, 280, 670, 150, 190, 310, 400 respectively. Based on the given information, answer the given sub-questions:
At what price do the top 25% of snack packets start? (More than one option can be correct)
**Options:**
*   6406533776848. It corresponds to the third quartile. (Correct)
*   6406533776849. 450 Rupees. (Correct)
*   6406533776850. It corresponds to the first quartile.
*   6406533776851. 190 Rupees.

**Solution Breakdown:**

1.  **Understand the Question:** "At what price do the top 25% of snack packets start?" This is asking for the value that separates the top 25% from the bottom 75%. This is the definition of the **third quartile ($Q_3$) or the 75th percentile ($P_{75}$)**. So, **Option 1 is true.**

2.  **Order the Dataset:**
    Prices: $\{120, 450, 620, 200, 280, 670, 150, 190, 310, 400\}$
    Sorted Prices: $\{120, 150, 190, 200, 280, 310, 400, 450, 620, 670\}$
    Number of data points ($n$) = 10.

3.  **Calculate $Q_3$ (75th Percentile):**
    For the P-th percentile position, calculate $L = \frac{P}{100} \times n$.
    For $P_{75}$, $L = \frac{75}{100} \times 10 = 7.5$.
    Since $L$ is not a whole number, round up to the next integer to find the position. Position = 8.
    The 8th value in the ordered list is 450.
    So, $Q_3 = 450$.

4.  **Evaluate Options:**
    *   Option 1: "It corresponds to the third quartile." -> **True.**
    *   Option 2: "450 Rupees." -> **True.**
    *   Option 3: "It corresponds to the first quartile." (First quartile is $Q_1$, which is $P_{25}$. $L = \frac{25}{100} \times 10 = 2.5 \implies$ 3rd position, which is 190. So this option is false).
    *   Option 4: "190 Rupees." (This is $Q_1$, not $Q_3$). -> **False.**

**Correct Answer (Q82): Options 6406533776848 and 6406533776849**

---

**Question 83 (Feb 2025 QDF2)**
**Question ID:** 6406531114691
**Question Label:** Short Answer Question
**Problem Statement:**
What is the Interquartile Range (IQR) of the snack packet prices?
(Prices: 120, 450, 620, 200, 280, 670, 150, 190, 310, 400)

**Solution Breakdown:**

1.  **Ordered Data (from Q82):** $\{120, 150, 190, 200, 280, 310, 400, 450, 620, 670\}$
    $n = 10$.

2.  **Calculate $Q_1$ (First Quartile / 25th Percentile):**
    Position for $P_{25}$: $L = \frac{25}{100} \times 10 = 2.5$.
    Round up to 3. The 3rd value is 190. So, $Q_1 = 190$.

3.  **Calculate $Q_3$ (Third Quartile / 75th Percentile):**
    Position for $P_{75}$: $L = \frac{75}{100} \times 10 = 7.5$.
    Round up to 8. The 8th value is 450. So, $Q_3 = 450$.

4.  **Calculate IQR:**
    IQR = $Q_3 - Q_1 = 450 - 190 = 260$.

**Correct Answer (Q83): 260**

---

**Question 86 (Feb 2025 QDF2)**
**Question ID:** 6406531114696
**Question Label:** Short Answer Question
**Problem Statement:**
The monthly salaries (in thousands) offered to employees in a company are represented in the following stem-and-leaf plot:
Stem | Leaf
--- | ---
1 | 2 4 6
2 | 0 2 4
3 | 1 2 6
Here, 5|2 represents 52.
What is the average monthly salary of the employees if each observation is increased by 3 and then multiplied by 2?

**Solution Breakdown:**

1.  **List Original Salaries from Stem-and-Leaf Plot:**
    *   Stem 1: 12, 14, 16 (representing 12,000, 14,000, 16,000)
    *   Stem 2: 20, 22, 24 (representing 20,000, 22,000, 24,000)
    *   Stem 3: 31, 32, 36 (representing 31,000, 32,000, 36,000)
    Original dataset $X = \{12, 14, 16, 20, 22, 24, 31, 32, 36\}$.
    Number of observations ($n$) = 9.

2.  **Calculate Mean of Original Salaries ($\bar{X}$):**
    $\bar{X} = \frac{12+14+16+20+22+24+31+32+36}{9} = \frac{207}{9} = 23$.

3.  **Analyze the Transformation:**
    Each observation is first "increased by 3" and then "multiplied by 2."
    This is a linear transformation: $Y = 2(X + 3) = 2X + 6$.
    So, $a=2$ and $b=6$.

4.  **Apply Property of Mean under Linear Transformation:**
    If $Y = aX + b$, then $\bar{Y} = a\bar{X} + b$.
    $\bar{Y} = 2 \times \bar{X} + 6$
    $\bar{Y} = 2 \times 23 + 6$
    $\bar{Y} = 46 + 6 = 52$.

**Correct Answer (Q86): 52**

---

**Question 87 (Feb 2025 QDF2)**
**Question ID:** 6406531114697
**Question Label:** Short Answer Question
**Problem Statement:**
What is the population variance of the given data if 10 is added to each observation?
(Stem and Leaf plot from Q86, representing salaries)

**Solution Breakdown:**

1.  **Original Salaries (Population) from Q86:** $X = \{12, 14, 16, 20, 22, 24, 31, 32, 36\}$.
    Number of observations ($N$) = 9.
    (Assuming this is the population as implied by "population variance").

2.  **Calculate Mean of Original Salaries ($\mu_X$):**
    $\mu_X = 23$ (from Q86 solution).

3.  **Calculate Population Variance of Original Salaries ($\sigma_X^2$):**
    $\sigma_X^2 = \frac{\sum (x_i - \mu_X)^2}{N}$
    Deviations from mean:
    $(12-23)^2 = (-11)^2 = 121$
    $(14-23)^2 = (-9)^2 = 81$
    $(16-23)^2 = (-7)^2 = 49$
    $(20-23)^2 = (-3)^2 = 9$
    $(22-23)^2 = (-1)^2 = 1$
    $(24-23)^2 = (1)^2 = 1$
    $(31-23)^2 = (8)^2 = 64$
    $(32-23)^2 = (9)^2 = 81$
    $(36-23)^2 = (13)^2 = 169$
    Sum of squared deviations $= 121+81+49+9+1+1+64+81+169 = 576$.
    $\sigma_X^2 = \frac{576}{9} = 64$.

4.  **Analyze the Transformation:**
    "10 is added to each observation."
    This is a linear transformation: $Y = X + 10$. So, $a=1$ and $b=10$.

5.  **Apply Property of Variance under Linear Transformation:**
    If $Y = aX + b$, then $\text{Var}(Y) = a^2 \cdot \text{Var}(X)$.
    Variance of Modified Data ($\sigma_Y^2$) = $(1)^2 \times \sigma_X^2$
    $\sigma_Y^2 = 1 \times 64 = 64$.
    Adding a constant only shifts the data, it does not change its spread.

**Correct Answer (Q87): 64**

---

**Question 102 (Feb 2025 QDF2)**
**Question ID:** 640653991852
**Question Label:** Short Answer Question
**Problem Statement:**
Please answer the subquestions based on the given stem-and-leaf plot:
Stem | Leaf
--- | ---
1 | 2 4 5
2 | 0 3 4 5
3 | 1 5 5 7
4 | 0 4 6
Here 1 | 5 represents 15.
What is the median of the data set represented by the stem-and-leaf plot?

**Solution Breakdown:**

1.  **List all data points from the Stem-and-Leaf Plot:**
    *   Stem 1: 12, 14, 15
    *   Stem 2: 20, 23, 24, 25
    *   Stem 3: 31, 35, 35, 37
    *   Stem 4: 40, 44, 46
    Ordered data set: $\{12, 14, 15, 20, 23, 24, 25, 31, 35, 35, 37, 40, 44, 46\}$

2.  **Count the number of observations (n):** There are 14 data points.

3.  **Find the Median (since n is even):**
    The median is the average of the two middle values, at positions $\frac{n}{2}$ and $\frac{n}{2}+1$.
    $\frac{14}{2} = 7$-th position.
    $\frac{14}{2} + 1 = 8$-th position.
    The 7th value is 25.
    The 8th value is 31.
    Median = $\frac{25 + 31}{2} = \frac{56}{2} = 28$.

**Correct Answer (Q102): 28**

---

**Question 103 (Feb 2025 QDF2)**
**Question ID:** 640653991853
**Question Label:** Short Answer Question
**Problem Statement:**
Calculate the range of the data set.
(Stem and Leaf plot from Q102)

**Solution Breakdown:**

1.  **Ordered Data (from Q102):** $\{12, 14, 15, 20, 23, 24, 25, 31, 35, 35, 37, 40, 44, 46\}$
2.  **Identify Maximum and Minimum Values:**
    *   Maximum Value = 46
    *   Minimum Value = 12
3.  **Calculate Range:**
    Range = Maximum Value - Minimum Value
    Range = $46 - 12 = 34$.

**Correct Answer (Q103): 34**

---

**Question 111 (Feb 2025 QDF2)**
**Question ID:** 640653991854
**Question Label:** Short Answer Question
**Problem Statement:**
In an exam, students' scores have an interquartile range (IQR) of 20. The teacher decides to first add 5 marks to each student's score and then multiply each adjusted score by 2. What will be the interquartile range now?

**Solution Breakdown:**

1.  **Original IQR:** $\text{IQR}_{original} = 20$.
2.  **Analyze the Transformation:**
    Each score ($X$) is transformed to a new score ($Y$) by:
    *   First, adding 5: $X' = X + 5$.
    *   Then, multiplying by 2: $Y = 2X'$.
    Combining these: $Y = 2(X+5) = 2X + 10$.
    This is a linear transformation $Y = aX + b$, with $a=2$ and $b=10$.

3.  **Apply Property of IQR under Linear Transformation:**
    If $Y = aX + b$, then $\text{IQR}(Y) = |a| \cdot \text{IQR}(X)$.
    The additive constant ($b$) does not affect measures of spread like IQR. The multiplicative constant ($a$) scales the spread.
    New IQR = $|2| \times \text{IQR}_{original}$
    New IQR = $2 \times 20 = 40$.

**Correct Answer (Q111): 40**

---
# WEEK 4: Association Between Two Variables

This week explores relationships between two variables, covering visual displays like scatterplots and numerical measures like covariance and correlation. These tools help us understand if variables tend to change together and the nature of that relationship.

## 4.1 Association Between Two Categorical Variables

### 4.1.1 Contingency Tables (Two-Way Tables)

*   **Purpose:** Display joint frequencies of two categorical variables.
*   **Components:**
    *   **Joint Frequencies:** Counts in the inner cells (e.g., number of males who prefer coffee).
    *   **Marginal Frequencies:** Totals for each row/column (e.g., total males, total coffee drinkers).
    *   **Grand Total:** Overall sum.
*   **Relative Frequencies:**
    *   **Joint:** Cell count / Grand Total.
    *   **Marginal:** Row/Column Total / Grand Total.
    *   **Conditional:** Cell count / Relevant Row/Column Total (e.g., proportion of coffee drinkers *among males* = $\frac{\text{Males who prefer Coffee}}{\text{Total Males}}$). Conditional frequencies are key for assessing association.

## 4.2 Association Between Two Numerical Variables

### 4.2.1 Scatterplot

*   **Purpose:** Visualizes the relationship between two numerical variables. Each pair of $(x,y)$ values is a point.
*   **Interpretation:** Look for:
    *   **Direction:** Positive (upward slope), Negative (downward slope), No direction.
    *   **Form:** Linear (straight line), Non-linear (curved).
    *   **Strength:** How tightly points cluster around the form (strong, moderate, weak).
    *   **Outliers:** Points far from the main cluster.

### 4.2.2 Covariance

*   **Definition:** Measures the extent to which two variables change together linearly.
*   **Formula (Population):** $\sigma_{XY} = \frac{\sum (x_i - \mu_X)(y_i - \mu_Y)}{N}$
*   **Formula (Sample):** $s_{XY} = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{n-1}$
*   **Interpretation:**
    *   Positive: Variables tend to increase/decrease together.
    *   Negative: As one increases, the other tends to decrease.
    *   Close to zero: Weak or no *linear* relationship.
*   **Limitation:** Magnitude depends on units, so it's not standardized.

### 4.2.3 Pearson Correlation Coefficient ($r$ or $\rho$)

*   **Definition:** A standardized measure of the *strength and direction of the linear relationship* between two numerical variables.
*   **Formula (Population):** $\rho = \frac{\sigma_{XY}}{\sigma_X \sigma_Y}$
*   **Formula (Sample):** $r = \frac{s_{XY}}{s_X s_Y}$
*   **Range:** -1 to +1.
*   **Interpretation:**
    *   $r = +1$: Perfect positive linear correlation.
    *   $r = -1$: Perfect negative linear correlation.
    *   $r = 0$: No linear correlation.
    *   Closer to $\pm 1$: Stronger linear relationship.
*   **Crucial Reminder:** **Correlation does not imply causation.** A strong correlation just means variables move together, not that one causes the other.

## Pattern 4.1: Analyzing Contingency Tables and Conditional Frequencies

These questions require you to interpret two-way tables and calculate proportions based on specific conditions.

---

**Question 74 (July 2024 QDF4)**
**Question ID:** 640653827223
**Question Label:** Multiple Choice Question
**Problem Statement:**
Amit took a survey of a group of 32 college going students (consisting only of male and female students) to know whether they own a smartphone or not and he got to know the following information.
(i). There are 3 males who do not own a smartphone.
(ii). There are total 27 females.
(iii). There are total 26 students who do not own a smartphone.
Create a two-way contingency table and find out the number of males in this group who own a smartphone?
**Options:**
*   6406532780453. 0
*   6406532780454. 2 (Correct)
*   6406532780455. 3
*   6406532780456. 4

**Solution Breakdown:**

1.  **Set up the Contingency Table:**

    |                | Smartphone | No Smartphone | Total |
    | :------------- | :--------- | :------------ | :---- |
    | **Male**       |            |               |       |
    | **Female**     |            |               |       |
    | **Total**      |            |               |       |

2.  **Fill in Knowns:**
    *   Total students = 32 (Grand Total).
    *   (i) 3 males do not own a smartphone.
    *   (ii) Total females = 27 (Female row total).
    *   (iii) Total students who do not own a smartphone = 26 (No Smartphone column total).

    |                | Smartphone | No Smartphone | Total |
    | :------------- | :--------- | :------------ | :---- |
    | **Male**       |            | 3             |       |
    | **Female**     |            |               | 27    |
    | **Total**      |            | 26            | 32    |

3.  **Deduce Missing Values:**
    *   **Total Males:** Total Students - Total Females = $32 - 27 = 5$.
    *   **Females who do not own smartphone:** Total "No Smartphone" - Males "No Smartphone" = $26 - 3 = 23$.
    *   **Females who own smartphone:** Total Females - Females "No Smartphone" = $27 - 23 = 4$.
    *   **Total students who own smartphone:** Total Students - Total "No Smartphone" = $32 - 26 = 6$.
    *   **Males who own smartphone (The question's target):** Total Males - Males "No Smartphone" = $5 - 3 = 2$.
    *   Alternatively: Total "Smartphone" - Females "Smartphone" = $6 - 4 = 2$.

4.  **Completed Table:**

    |                | Smartphone | No Smartphone | Total |
    | :------------- | :--------- | :------------ | :---- |
    | **Male**       | **2**      | 3             | 5     |
    | **Female**     | 4          | 23            | 27    |
    | **Total**      | 6          | 26            | 32    |

**Correct Answer (Q74): 2**

---

**Question 75 (July 2024 QDF4)**
**Question ID:** 640653827224
**Question Label:** Multiple Select Question
**Problem Statement:**
(Using the same survey data from Q74)
Which of the following option(s) is (are) true?
**Options:**
*   6406532780457. There are 40% of the males who do not own a smartphone.
*   6406532780458. There are 14.81% of the females who own a smartphone. (Correct)
*   6406532780459. 18.75% of the total students own a smartphone. (Correct)
*   6406532780460. We can calculate covariance to find the association between "Gender" and "Ownership of the smartphone”.

**Solution Breakdown:**

1.  **Refer to Completed Contingency Table (from Q74):**

    |                | Smartphone | No Smartphone | Total |
    | :------------- | :--------- | :------------ | :---- |
    | **Male**       | 2          | 3             | 5     |
    | **Female**     | 4          | 23            | 27    |
    | **Total**      | 6          | 26            | 32    |

2.  **Statement 1: "There are 40% of the males who do not own a smartphone."**
    *   Males who do not own smartphone = 3.
    *   Total Males = 5.
    *   Percentage = $\frac{3}{5} \times 100\% = 0.6 \times 100\% = 60\%$.
    *   **Truth Value:** False (It says 40%).

3.  **Statement 2: "There are 14.81% of the females who own a smartphone."**
    *   Females who own smartphone = 4.
    *   Total Females = 27.
    *   Percentage = $\frac{4}{27} \times 100\% \approx 0.148148... \times 100\% \approx 14.81\%$.
    *   **Truth Value:** True.

4.  **Statement 3: "18.75% of the total students own a smartphone."**
    *   Total students who own smartphone = 6.
    *   Total students = 32.
    *   Percentage = $\frac{6}{32} \times 100\% = \frac{3}{16} \times 100\% = 0.1875 \times 100\% = 18.75\%$.
    *   **Truth Value:** True.

5.  **Statement 4: "We can calculate covariance to find the association between "Gender" and "Ownership of the smartphone”."**
    *   **Gender:** Categorical (Nominal).
    *   **Ownership of smartphone:** Categorical (Nominal/Binary).
    *   **Covariance:** A measure of linear association specifically for *two numerical variables*.
    *   **Analysis:** You cannot calculate covariance between two categorical variables. For categorical variables, you use contingency tables and conditional probabilities to show association.
    *   **Truth Value:** False.

**Correct Answer (Q75): Options 6406532780458 and 6406532780459**

---

**Question 75 (Feb 2025 QDF2)**
**Question ID:** 6406531114682
**Question Label:** Multiple Choice Question
**Problem Statement:**
A study was conducted to investigate the association between smoking habits and lung disease within a population. The collected data is presented in Table Q.3.
Have Lung Disease | Do Not Have Lung Disease | Total
--- | --- | ---
**Smoker** | 40 | x | 100
**Non-Smoker** | y | 180 | 200
**Total** | 60 | 240 | 300
What proportion of non-smokers have lung disease?
**Options:**
*   6406533776823. 0.10 (Correct)
*   6406533776824. 0.60
*   6406533776825. 0.20
*   6406533776826. 0.30

**Solution Breakdown:**

1.  **Identify the Question:** "What proportion of **non-smokers** have lung disease?" This is a **conditional proportion/probability**. The condition is "non-smoker."
2.  **Locate Relevant Data:**
    *   Number of non-smokers who have lung disease = `y`.
    *   Total non-smokers = 200.
    *   From the table, Total "Have Lung Disease" = 60. Smoker "Have Lung Disease" = 40.
    *   So, `y` = Total "Have Lung Disease" - Smoker "Have Lung Disease" = $60 - 40 = 20$.
3.  **Calculate the Proportion:**
    Proportion = $\frac{\text{Non-smokers who have Lung Disease}}{\text{Total Non-Smokers}}$
    Proportion = $\frac{20}{200} = 0.10$.

**Correct Answer (Q75): 0.10**

---

## Pattern 4.2: Interpreting Scatterplots and Calculating Covariance/Correlation

These questions assess your ability to visualize linear relationships and quantify them using covariance and correlation.

---

**Question 78 (July 2024 QDF4)**
**Question ID:** 640653827225
**Question Label:** Multiple Choice Question
**Problem Statement:**
Consider the following four images of the Scatter plot.
(Images of scatter plots A, B, C, D)
Please select the option that will represent the correlation values arranged in ascending order.
**Options:**
*   6406532780461. A<B<C<D
*   6406532780462. B <C<D<A (Correct)
*   6406532780463. B < A<C<D
*   6406532780464. A < D<C<B

**Solution Breakdown:**

1.  **Analyze each Scatterplot (visual interpretation of correlation):**
    *   **Correlation ranges from -1 to +1.**
    *   **Closer to 1 or -1:** Stronger linear relationship.
    *   **Positive slope:** Positive correlation.
    *   **Negative slope:** Negative correlation.
    *   **No clear slope:** Near zero correlation.

    *   **Plot A:** Points are tightly clustered along a clear **positive** linear trend. This indicates a very strong positive correlation, close to +1. (e.g., $r \approx 0.9$)
    *   **Plot B:** Points are tightly clustered along a clear **negative** linear trend. This indicates a very strong negative correlation, close to -1. (e.g., $r \approx -0.9$)
    *   **Plot C:** Points are scattered with no clear linear trend. This indicates a very weak or no linear correlation, close to 0. (e.g., $r \approx 0.1$)
    *   **Plot D:** Points show a clear **positive** linear trend, but they are more spread out than in Plot A. This indicates a moderate to strong positive correlation, but less than A. (e.g., $r \approx 0.6$)

2.  **Assign approximate correlation values (conceptual):**
    *   $r_A \approx 0.9$
    *   $r_B \approx -0.9$
    *   $r_C \approx 0.1$
    *   $r_D \approx 0.6$

3.  **Arrange in Ascending Order (Smallest to Largest):**
    Negative values are smaller than positive values.
    $-0.9 < 0.1 < 0.6 < 0.9$
    So, $r_B < r_C < r_D < r_A$.

**Correct Answer (Q78): Option 6406532780462 (B < C < D < A)**

---

**Question 80 (July 2024 QDF4)**
**Question ID:** 640653827226
**Question Label:** Short Answer Question
**Problem Statement:**
Find the population covariance between X and Y for the dataset given in Table Q.2.
X | -3 | -4 | -5 | 5 | 4 | 3
--- | --- | --- | --- | --- | --- | ---
Y | 10 | 5 | 3 | 3 | 5 | 10

**Solution Breakdown:**

1.  **List Data Pairs:**
    $(x_i, y_i)$: $(-3, 10), (-4, 5), (-5, 3), (5, 3), (4, 5), (3, 10)$
    Number of data points ($N$) = 6. (Assuming population as asked for population covariance).

2.  **Calculate Mean of X ($\mu_X$):**
    $\mu_X = \frac{-3 + (-4) + (-5) + 5 + 4 + 3}{6} = \frac{0}{6} = 0$.

3.  **Calculate Mean of Y ($\mu_Y$):**
    $\mu_Y = \frac{10 + 5 + 3 + 3 + 5 + 10}{6} = \frac{36}{6} = 6$.

4.  **Calculate Covariance ($\sigma_{XY}$):**
    $\sigma_{XY} = \frac{\sum (x_i - \mu_X)(y_i - \mu_Y)}{N}$
    Since $\mu_X = 0$, $(x_i - \mu_X)$ simplifies to $x_i$.
    $(x_i - \mu_X)(y_i - \mu_Y)$ terms:
    *   $(-3 - 0)(10 - 6) = (-3)(4) = -12$
    *   $(-4 - 0)(5 - 6) = (-4)(-1) = 4$
    *   $(-5 - 0)(3 - 6) = (-5)(-3) = 15$
    *   $(5 - 0)(3 - 6) = (5)(-3) = -15$
    *   $(4 - 0)(5 - 6) = (4)(-1) = -4$
    *   $(3 - 0)(10 - 6) = (3)(4) = 12$
    Sum of products of deviations $= -12 + 4 + 15 - 15 - 4 + 12 = 0$.
    $\sigma_{XY} = \frac{0}{6} = 0$.

**Correct Answer (Q80): 0**

---

**Question 83 (July 2024 QDF4)**
**Question ID:** 640653827218
**Question Label:** Short Answer Question
**Problem Statement:**
Calculate the correlation coefficient between the marks scored by Manoj and Nitin.
(Manoj's marks: 60, 70, 65, 75, 80; Nitin scored 5 marks more than Manoj in each subject).

**Solution Breakdown:**

1.  **Manoj's Marks (X):** $X = \{60, 70, 65, 75, 80\}$.
2.  **Nitin's Marks (Y):** Nitin's marks are $Y = X + 5$, so $Y = \{65, 75, 70, 80, 85\}$.
3.  **Understanding the Relationship:** Since Nitin's marks are consistently 5 points higher than Manoj's for *each* subject, there is a perfect linear relationship between their scores. When one goes up by a certain amount, the other goes up by exactly the same amount relative to its own baseline.
    *   This implies a perfect positive linear correlation.
    *   A perfect positive linear correlation always results in a Pearson correlation coefficient of +1.

4.  **Formal Calculation (Optional, but good for verification):**
    *   $\bar{X} = 70$ (from Q81).
    *   $\bar{Y} = 75$ (from Q81).
    *   **Sample Standard Deviation of X ($s_X$):**
        *   $s_X^2 = \frac{\sum (x_i - \bar{x})^2}{n-1} = \frac{(60-70)^2+(70-70)^2+(65-70)^2+(75-70)^2+(80-70)^2}{5-1}$
        *   $s_X^2 = \frac{(-10)^2 + 0^2 + (-5)^2 + 5^2 + 10^2}{4} = \frac{100+0+25+25+100}{4} = \frac{250}{4} = 62.5$.
        *   $s_X = \sqrt{62.5} \approx 7.9057$.
    *   **Sample Standard Deviation of Y ($s_Y$):**
        *   Since $Y = X + 5$, $s_Y = s_X$ (adding a constant doesn't change spread). So $s_Y \approx 7.9057$.
    *   **Sample Covariance ($s_{XY}$):**
        $s_{XY} = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{n-1}$
        Terms $(x_i - \bar{x})(y_i - \bar{y})$:
        *   $(60-70)(65-75) = (-10)(-10) = 100$
        *   $(70-70)(75-75) = (0)(0) = 0$
        *   $(65-70)(70-75) = (-5)(-5) = 25$
        *   $(75-70)(80-85) = (5)(5) = 25$
        *   $(80-70)(85-85) = (10)(10) = 100$
        Sum of products of deviations $= 100 + 0 + 25 + 25 + 100 = 250$.
        $s_{XY} = \frac{250}{4} = 62.5$.
    *   **Pearson Correlation Coefficient ($r$):**
        $r = \frac{s_{XY}}{s_X s_Y} = \frac{62.5}{\sqrt{62.5} \times \sqrt{62.5}} = \frac{62.5}{62.5} = 1$.

**Correct Answer (Q83): 1**

---

**Question 81 (Feb 2025 QDF2)**
**Question ID:** 6406531114688
**Question Label:** Short Answer Question
**Problem Statement:**
A researcher collected data on the amount of fertilizer (in kilograms) applied and the crop yield (in kilograms per hectare) for 5 different fields. The data is summarized in Table Q.2.
X: Fertilizer Applied (kg) | Y: Crop Yield (kg/hectare)
--- | ---
2 | 30
3 | 35
4 | 45
5 | 50
6 | 60
Calculate population covariance between X and Y.

**Solution Breakdown:**

1.  **List Data Pairs:**
    $(x_i, y_i)$: $(2, 30), (3, 35), (4, 45), (5, 50), (6, 60)$
    Number of data points ($N$) = 5 (assuming population as asked).

2.  **Calculate Mean of X ($\mu_X$):**
    $\mu_X = \frac{2 + 3 + 4 + 5 + 6}{5} = \frac{20}{5} = 4$.

3.  **Calculate Mean of Y ($\mu_Y$):**
    $\mu_Y = \frac{30 + 35 + 45 + 50 + 60}{5} = \frac{220}{5} = 44$.

4.  **Calculate Covariance ($\sigma_{XY}$):**
    $\sigma_{XY} = \frac{\sum (x_i - \mu_X)(y_i - \mu_Y)}{N}$
    $(x_i - \mu_X)(y_i - \mu_Y)$ terms:
    *   $(2 - 4)(30 - 44) = (-2)(-14) = 28$
    *   $(3 - 4)(35 - 44) = (-1)(-9) = 9$
    *   $(4 - 4)(45 - 44) = (0)(1) = 0$
    *   $(5 - 4)(50 - 44) = (1)(6) = 6$
    *   $(6 - 4)(60 - 44) = (2)(16) = 32$
    Sum of products of deviations $= 28 + 9 + 0 + 6 + 32 = 75$.
    $\sigma_{XY} = \frac{75}{5} = 15$.

**Correct Answer (Q81): 15**

---

**Question 106 (Feb 2025 QDF2)**
**Question ID:** 640653991856
**Question Label:** Short Answer Question
**Problem Statement:**
Find the sample covariance between X and Y for the dataset given in Table 2.
X | -5 | -4 | -3 | 3 | 4 | 5
--- | --- | --- | --- | --- | --- | ---
Y | -13 | -12 | -5 | 13 | 12 | 5

**Solution Breakdown:**

1.  **List Data Pairs:**
    $(x_i, y_i)$: $(-5, -13), (-4, -12), (-3, -5), (3, 13), (4, 12), (5, 5)$
    Number of data points ($n$) = 6. (Asking for sample covariance).

2.  **Calculate Sample Mean of X ($\bar{x}$):**
    $\bar{x} = \frac{-5 + (-4) + (-3) + 3 + 4 + 5}{6} = \frac{0}{6} = 0$.

3.  **Calculate Sample Mean of Y ($\bar{y}$):**
    $\bar{y} = \frac{-13 + (-12) + (-5) + 13 + 12 + 5}{6} = \frac{0}{6} = 0$.

4.  **Calculate Sample Covariance ($s_{XY}$):**
    $s_{XY} = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{n-1}$
    Since $\bar{x}=0$ and $\bar{y}=0$, $(x_i - \bar{x})$ becomes $x_i$ and $(y_i - \bar{y})$ becomes $y_i$.
    Terms $x_i y_i$:
    *   $(-5)(-13) = 65$
    *   $(-4)(-12) = 48$
    *   $(-3)(-5) = 15$
    *   $(3)(13) = 39$
    *   $(4)(12) = 48$
    *   $(5)(5) = 25$
    Sum of products $= 65 + 48 + 15 + 39 + 48 + 25 = 240$.
    $n-1 = 6-1 = 5$.
    $s_{XY} = \frac{240}{5} = 48$.

**Correct Answer (Q106): 48**

---

**Question 107 (Feb 2025 QDF2)**
**Question ID:** 640653991857
**Question Label:** Short Answer Question
**Problem Statement:**
Find the sample correlation coefficient(r) between X and Y for the dataset given in Table 2. (Write correct upto 3 digits after the decimal)
(Data from Q106)

**Solution Breakdown:**

1.  **From Q106:**
    *   $s_{XY} = 48$.
    *   $\bar{x} = 0, \bar{y} = 0$.
    *   Data pairs: $(-5, -13), (-4, -12), (-3, -5), (3, 13), (4, 12), (5, 5)$

2.  **Calculate Sample Standard Deviation of X ($s_X$):**
    $s_X^2 = \frac{\sum (x_i - \bar{x})^2}{n-1} = \frac{\sum x_i^2}{n-1}$ (since $\bar{x}=0$)
    $\sum x_i^2 = (-5)^2 + (-4)^2 + (-3)^2 + 3^2 + 4^2 + 5^2$
    $= 25 + 16 + 9 + 9 + 16 + 25 = 100$.
    $s_X^2 = \frac{100}{5} = 20$.
    $s_X = \sqrt{20} \approx 4.4721$.

3.  **Calculate Sample Standard Deviation of Y ($s_Y$):**
    $s_Y^2 = \frac{\sum (y_i - \bar{y})^2}{n-1} = \frac{\sum y_i^2}{n-1}$ (since $\bar{y}=0$)
    $\sum y_i^2 = (-13)^2 + (-12)^2 + (-5)^2 + 13^2 + 12^2 + 5^2$
    $= 169 + 144 + 25 + 169 + 144 + 25 = 676$.
    $s_Y^2 = \frac{676}{5} = 135.2$.
    $s_Y = \sqrt{135.2} \approx 11.6276$.

4.  **Calculate Pearson Correlation Coefficient ($r$):**
    $r = \frac{s_{XY}}{s_X s_Y} = \frac{48}{\sqrt{20} \times \sqrt{135.2}} = \frac{48}{\sqrt{20 \times 135.2}} = \frac{48}{\sqrt{2704}} = \frac{48}{52}$.
    $r = \frac{48}{52} = \frac{12}{13} \approx 0.923076...$
    Correct to 3 digits after the decimal: $0.923$.

**Correct Answer (Q107): 0.923 (or within range 0.921 to 0.925)**

---

