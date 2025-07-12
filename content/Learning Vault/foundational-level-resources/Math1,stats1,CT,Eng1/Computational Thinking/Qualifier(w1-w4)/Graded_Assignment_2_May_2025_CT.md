# Graded Assignment- 2 - (May 2025 - CT)

> The due date for submitting this assignment has passed.
Due on 2025-06-18, 23:59 IST.
You may submit any number of times before the due date. The final submission will be considered for grading.

> **Last Submitted:** You have last submitted on: 2025-06-11, 21:32 IST

---

### Question 1

The following procedure counts the number of students from Bengaluru whose total marks are less than the average total marks from the “Scores” dataset and stores it in variable A. Let avgT be the average total marks. The programmer may have made mistakes in one or more steps. Identify all such steps (if any). It is a Multiple Select Question (MSQ).

Step 1 : Arrange all cards in a single pile called **Pile 1**

Step 2 : Initialize variable **A** to 0

Step 3 : If **Pile 1** is empty then stop the iteration

Step 4 : Read the top card in **Pile 1**

Step 5 : If X.CityTown == “Bengaluru” and X.Total > avgT then add 1 to **A**

Step 6 : Move the current card to another pile called **Pile 2** and repeat from **Step 2**
- [ ] Step 5
- [x] Step 6
- [ ] Step 2
- [ ] Step 3
- [ ] No mistake


**Accepted Answers:**

* Step 5
* Step 6

---

### Question 2

At the end of the execution of the given procedure on the “Scores” dataset, what will **A** and **B** represent? (MCQ)

  

Step 1. Arrange all cards in a single pile called **Pile 1**  
Step 2. Maintain two variables **A, B** and initialize **A** to 101 and **B** to 0.  
Step 3. If **Pile 1** is empty then stop the iteration  
Step 4. Read the top card in **Pile 1**  
Step 5. If **A** > _Chemistry marks_ , then store _Chemistry marks_ in **A**  
Step 6. If **B** < _Mathematics marks_, then store _Mathematics marks_ in **B**  
Step 7. Move the current card to another pile called **Pile 2** and repeat from **Step 3**
- [x] **A** = Lowest marks in Chemistry, **B** = Highest marks in Mathematics
- [ ] **A** = Highest marks in Chemistry, **B** = Lowest marks in Mathematics
- [ ] **A** = Lowest marks in Chemistry, **B** = 0
- [ ] **A** = 101, **B** = Lowest marks in Mathematics

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* **A** = Lowest marks in Chemistry, **B** = Highest marks in Mathematics

---

### Question 3

The following procedure took data from the “Scores” dataset and **A** represents the number of male students whose Physics marks are less than the Mathematics marks but equal to their Chemistry marks. The programmer may have made mistakes in one or more steps. Identify all such steps (if any). It is a Multiple Select Question (MSQ).

Step 1 : Arrange all cards in a single pile called **Pile 1**

Step 2 : Initialize variable **A** to 1

Step 3 : If **Pile 1** is empty then stop the iteration

Step 4 : Read the top card in **Pile 1**

Step 5 : If Gender is ‘M’ and _Physics marks_ = _Mathematics marks_ and _Chemistry marks_ > _Physics marks_ then add 1 to **A**

Step 6 : Move the current card to another pile called **Pile 2** and repeat from **Step 3**
- [ ] Step 2
- [x] Step 5
- [ ] Step 6
- [ ] No mistake


**Accepted Answers:**

* Step 2
* Step 5

---

### Question 4

At the end of the execution of the given procedure on the “Words” dataset, what will **A** represent? This is a Multiple Choice Question (MCQ)

Step 1. Arrange all cards in a single pile called **Pile 1**

Step 2. Maintain two variables **A, B** and initialize **A** to 1000 and **B** to 0

Step 3. If **Pile 1** is empty then stop the iteration

Step 4. Read the top card in **Pile 1**

Step 5. Add _Letter Count_ to variable **B**

Step 6. If _Word_ does not end with a full stop then execute **Step 9**

Step 7. If _Word_ ends with a full stop and **B < A** then store **B** in **A**

Step 8. Re-initialize the variable **B** to 0

Step 9. Move the current card to another pile called **Pile 2** and repeat from **Step 3**
- [x] Length of the shortest sentence based on the number of words
- [ ] Length of the longest sentence based on the number of words
- [ ] Length of the longest sentence based on the number of letters
- [ ] Length of the shortest sentence based on the number of letters


**Accepted Answers:**

* Length of the shortest sentence based on the number of letters

---

### Question 5

Assume that **a, b,** and **c** are three distinct integers. What will **X** represent after the execution of the following procedure?

Step 1. Maintain variable **X** and Initialize it to 0

Step 2. If **a** < **b** then go to step 4

Step 3. If **b** < **c** then store b in **X** else store **c** in **X** and stop the procedure.

Step 4. If **a** < **c** then store a in **X** else store **c** in **X**
- [ ] Largest among **a**, **b**, and **c**
- [x] Smallest among **a**, **b** , and **c**
- [ ] **X** will always be 0
- [ ] Second smallest among **a**, **b**, and **c**

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* Smallest among **a**, **b** , and **c**

---

### Question 6

What will be the value of **X** after the execution of the following procedure using the “Scores” dataset? (MCQ)  
(Note: Consider the same sequence as given in the Scores datasets)  

  

Step 1: Arrange all cards in a single pile called **Pile 1**  
Step 2: Maintain variables **A, B, C, D, Y** and Initialize them all to 0 except **Y**. Initialize **Y** to 100  
Step 3: Maintain a variable **X** and initialize it to “None”  
Step 4: If **Pile 1** is empty then stop the iteration  
Step 5: Read the top card in **Pile 1**  
Step 6: If the Town/City is “Chennai” then add one to **A**. If **A < Y** then store **A** in **Y** and “Chennai” in **X**  
Step 7: If the Town/City is “Bengaluru” then add one to **B**. If **B < Y** then store **B** in **Y** and “Bengaluru” in **X**  
Step 8: If the Town/City is “Madurai” then add one to **C**. If **C < Y** then store **C** in **Y** and “Madurai” in **X**  
Step 9: If the Town/City is “Vellore” then add one to **D**. If **D < Y** then store **D** in **Y** and “Vellore” in **X**  
Step 10: Move the current card to another pile called **Pile 2** and repeat from **Step 4**
- [x] Chennai
- [ ] Bengaluru
- [ ] Madurai
- [ ] Vellore

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* Chennai

---

### Question 7

The following flowchart is executed using the “Scores” dataset. Assume that Rida and Siddharth both have scored the lowest total marks across the whole dataset which is 173. Let cards are arranged in such a way that Rida's card is below Siddharth's card, what will the values of **A** and **B** be at the end of the execution?  
  
![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/Screenshot%202024-01-22%20194658.png?seed=143&url=assets/img/Screenshot%202024-01-22%20194658.png)
- [ ] **A** \= "Siddharth", **B** = 173
- [x] **A** = 173 , **B** = "Rida"
- [ ] **A** = "Rida", **B** = 173
- [ ] **A** \= 173, **B** \= "Siddharth"

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* **A** = 173 , **B** = "Rida"

---

### Question 8

The following pseudocode is executed using the “Scores” dataset. What will **count** represent at the end of the execution of pseudocode?  
  
![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/w2ga.png?seed=96057&url=assets/img/w2ga.png)
- [ ] Number of students who scored less than 80 marks in at least two subjects
- [x] Number of students who scored more than 80 marks in exactly two subjects
- [ ] Number of students who scored more than 80 marks in all three subjects
- [ ] Number of students who scored less than 80 marks in at least one subject

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* Number of students who scored more than 80 marks in exactly two subjects

---

### Question 9

What will **(A–B)** represent after execution of the following procedure using the “Shopping Bills” dataset? (MCQ)

Step 1 : Arrange all cards in a single pile called **Pile 1**

Step 2 : Initialize variables **A** and **B** to 0

Step 3 : If **Pile 1** is empty then stop the iteration

Step 4 : Read the top card in **Pile 1**

Step 5 : If the bill contains an item “Bananas” then add 1 to variable **A**

Step 6 : If Total < 600 and the bill contains an item “Bananas” then add 1 to variable **B**

Step 7 : Move the current card to another pile called **Pile 2** and repeat from **Step 3**
- [x] Number of bills that contain the item "Bananas" and total is more than or equal to 600
- [ ] Number of bills that contain the item "Bananas" and total is less than 600
- [ ] Number of bills that do not contain the item "Bananas" and total is more than 600
- [ ] Number of bills that do not contain the item "Bananas" and total is less than 600

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* Number of bills that contain the item "Bananas" and total is more than or equal to 600

---

### Question 10

The given pseudocode is executed using the “Scores” dataset. At the end of the execution, **C** will be True if there are more female students from Chennai than male students from Bangalore. Choose the correct option to complete the pseudocode. (MCQ)  
  
![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/week%20102.png?seed=16432&url=assets/img/week%20102.png)
- [x] Statement 1: **A** = **A** + 1, Statement 2: **A** > **B**
- [ ] Statement 1: **A** = **A** - 1, Statement 2: **A** > **B**
- [ ] Statement 1: **A** = **A** + 1, Statement 2: **A** < **B**
- [ ] Statement 1: **A** = **A** - 1, Statement 2: **A** < **B**

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* Statement 1: **A** = **A** + 1, Statement 2: **A** > **B**

---

