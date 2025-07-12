# Graded Assignment - 3 - (May 2025 - CT)

> The due date for submitting this assignment has passed.
Due on 2025-06-25, 23:59 IST.
You may submit any number of times before the due date. The final submission will be considered for grading.

> **Last Submitted:** You have last submitted on: 2025-06-24, 21:25 IST

---

### Question 1

The following pseudocode is executed using the **"Library"** dataset.  
At the end of the execution, **N** captures the name of the book which has the maximum number of pages and is written in a language other than English, and **A** captures the number of pages in the book.  
  

A = 0, N = "None"

while(Table 1 has more rows){

    Read the first row X in Table 1

    if(X.Language != "English" and X.Pages > A){

        A = X.Pages

        N = X.Name

    }

    Move X to Table 2

}

  
Assume that the rows of the table are shuffled in any random order, choose the correct option(s).  
It is a **Multiple Select Question (MSQ)**.
- [ ] There might be some change in the values of both A and N, based on the order of rows
- [ ] There might be a change in the value of N, based on the order of rows
- [x] There will be NO change in the values of both A and N, based on the order of rows
- [ ] There might be a change in the value of A, based on the order of rows


**Accepted Answers:**

* There might be a change in the value of N, based on the order of rows

---

### Question 2

The following pseudocode is executed using the **“Scores”** dataset.  
What will **count** represent at the end of the execution?  
  

count = 0

while(Table 1 has more rows){

    Read the first row X in Table 1

    Move X to Table 2

    Flag = True

    while(Table 1 has more rows){

        Read the first row Y in Table 1

        if(X.Mathematics == Y.Mathematics){

            Flag = False

            Move Y to Table 2

        }

        else{

            Move Y to Table 3

        }

    }

    if(Flag){

        count = count + 1

    }

    Move all rows from Table 3 to Table 1

}
- [ ] Number of students with same Mathematics marks
- [ ] Number of pairs of students with same Mathematics marks
- [x] Number of students with distinct Mathematics marks
- [ ] Number of pairs of students with distinct Mathematics marks

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* Number of students with distinct Mathematics marks

---

### Question 3

The following pseudocode is executed using the “Scores” dataset.(MCQ)  
  
![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/question%203w3.png)  
  
At the end of the execution, **E** will be True if
- [ ] All female students have scores greater than or equal to 60 in either Physics, Chemistry or Maths
- [ ] All female students have scores less than 60 in either Physics, Chemistry or Maths
- [ ] There is at least one female student with scores less than 60 in Physics, Chemistry or Maths
- [x] All female students have scores greater than or equal to 60 in Physics, Chemistry and Maths

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* All female students have scores greater than or equal to 60 in Physics, Chemistry and Maths

---

### Question 4

The following pseudocode is executed using the “Shopping Bills” dataset. Procedure **checkShoppingBills** accepts a card **Y** and returns True if the minimum total bill amount of shop is greater than the average total bill amount of shop from where the card **Y** is generated otherwise returns False. Choose the correct code fragments to complete the procedure. It is a Multiple Select Question (MSQ). Note : **MAX\_VALUE** represent the maximum bill amount of shop **Y**.  
![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/ga3-4-1.png?seed=47693&url=assets/img/ga3-4-1.png)
- [ ] ![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/ga3-4-a.png?seed=71436&url=assets/img/ga3-4-a.png)
- [ ] ![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/3rdoption%204th%20question.png)
- [ ] ![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/q4opc.png?seed=97591&url=assets/img/q4opc.png)
- [x] ![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/option%204%20is%20correct.png?seed=67564&url=assets/img/option%204%20is%20correct.png)

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* ![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/option%204%20is%20correct.png?seed=67564&url=assets/img/option%204%20is%20correct.png)

---

### Question 5

The following pseudocode is executed using the "Scores" dataset. What will **A** represent at the end of the execution?(MCQ)  
  
![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/5week4.png?seed=94576&url=assets/img/5week4.png)
- [ ] Number of students scored above 60 in all three subjects
- [x] Number of students scored below 60 in at least any one subject
- [ ] **A** will always be 0
- [ ] Number of students scored exactly 60 in all three subjects

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* Number of students scored below 60 in at least any one subject

---

### Question 6

The following pseudocode is executed using the “Scores” dataset. At the end of the execution, variable **Count** captures the number of students whose total marks are more than the average (of total marks) of entire dataset but have scored below the subject average in any two subjects. Assume that the variable **AvgT** holds the value of the average total marks. Similarly, the variables **AvgP, AvgC** and **AvgM** hold the value of the average marks of Physics, Chemistry and Mathematics respectively. Choose the correct code fragment to complete the pseudocode.It is a Multiple Select Question(MSQ).  
  
![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/WEEK36Q.png?seed=22819&url=assets/img/WEEK36Q.png)
- [x] ![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/GS3-6A.png?seed=62677&url=assets/img/GS3-6A.png)
- [ ] ![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/optionb-6.png)
- [ ] ![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/GS3-6C.png?seed=8207&url=assets/img/GS3-6C.png)
- [ ] ![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/GS3-6D.png?seed=32818&url=assets/img/GS3-6D.png)

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* ![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/GS3-6A.png?seed=62677&url=assets/img/GS3-6A.png)

---

### Question 7

The following pseudocode is executed using the “Scores” dataset.(MCQ)  
![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/GA3-7.png?seed=89317&url=assets/img/GA3-7.png)  

At the end of the execution, **A** represents the number of students from Madurai having total marks.............
- [ ] greater than the average marks of students
- [ ] greater than the average marks of students from Vellore and Chennai
- [x] greater than the average marks of students from Vellore but less than that of Chennai
- [ ] greater than the average marks of students from Chennai but less than that of Vellore

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* greater than the average marks of students from Vellore but less than that of Chennai

---

### Question 8

The following pseudocode is executed using the "Scores" dataset. At the end of the execution, **A** captures the number of female students who are below average in at least one subject. Assume that the variables **M**, **P** and **C** hold the average marks of the subjects Mathematics, Physics and Chemistry respectively. The pseudocode may have mistakes. Identify all such mistakes (if any). Assume that all statements not listed in the options below are free of errors. It is a Multiple Select Question (MSQ).

  
![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/GS3-8.png?seed=39212&url=assets/img/GS3-8.png)  
  
.
- [ ] Line 1: Incorrect initialization of **A**
- [x] Line 3: Incorrect initialization of **B**
- [ ] Line 7: Incorrect Update of **B**
- [ ] Line 13: Incorrect Update of **B**
- [ ] No error in the code


**Accepted Answers:**

* Line 3: Incorrect initialization of **B**
* Line 7: Incorrect Update of **B**
* Line 13: Incorrect Update of **B**

---

### Question 9

The following pseudocode is executed using the “Scores” dataset. What will A represent at the end of the execution?   

(MCQ)  
![](https://backend.seek.study.iitm.ac.in/24t2_cs1001/assets/img/GA3Q9.png)
- [x] Number of students with highest marks only in Mathematics out of their three subjects' marks
- [ ] Number of students with highest marks only in Mathematics and lowest marks only in Physics
- [ ] Number of students with highest marks only in Chemistry out of their three subjects' marks
- [ ] Number of students with lowest marks only in Physics out of their three subjects' marks


**Accepted Answers:**

* Number of students with lowest marks only in Physics out of their three subjects' marks

---

### Question 10

The following pseudocode is executed using the “Words” dataset. What will **A** represent at the end of the execution?(MCQ)  
  
![](https://backend.seek.study.iitm.ac.in/24t1_cs1001/assets/img/GA3-10.png?seed=41614&url=assets/img/GA3-10.png)
- [ ] Number of words that end with a comma.
- [ ] Number of words that end with a comma and have a letter count greater than ratio of number of words to sum of letter count.
- [ ] Number of words that end with a comma and have a letter count less than or equal to the average letter count of dataset.
- [x] Number of words that end with a comma and have a letter count greater than the average letter count of dataset.

**Status:** Yes, the answer is correct.
**Score: 2**

**Accepted Answers:**

* Number of words that end with a comma and have a letter count greater than the average letter count of dataset.

---

