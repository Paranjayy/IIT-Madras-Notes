# Mock test 1 - (May 2025 - CT)

> This assignment will not be graded and is only for practice.

---

### Question 1

The following pseudocode is executed using the “Scores” dataset. What will **A** represent at the end of execution?

`   xxxxxxxxxx  1  A = 0   2  while(Table 1 has more rows){   3      Read the first row X in Table 1   4      if(X.Gender == 'M' and X.CityTown != “Chennai”){   5          A = A + X.Mathematics   6      }   7      Move X to Table 2   8  }       `
- [ ] Sum of Mathematics marks of students from Chennai
- [ ] Sum of Mathematics marks of male students from Chennai
- [ ] Sum of Mathematics marks of male students
- [ ] Sum of Mathematics marks of male students not from Chennai

---

### Question 2

Match the following expressions in the Column 1 with the appropriate values in column 2. table { border: 1px solid black; width: 100%; } th, td { text-align: left; font-size: 16px; padding: 8px; border: 1px solid black; } tr:nth-child(even) { background-color: #D6EEEE; } a { color: blue; }

Column 1

Column 2

a. 2 = 2 or 2 > 3

1\. Invalid expression

b. 2 == 2 and 2 > 3

2\. True

c. 2 = 3

3\. False

d. 2 + '2'

4\. 4

e. 2 >=2

5\. "22"
- [ ] a - (2), b - (3), c - (1), d - (1), e - (2)
- [ ] a - (1), b - (3), c - (1), d - (1), e - (2)
- [ ] a - (2), b - (3), c - (1), d - (4), e - (2)
- [ ] a - (1), b - (3), c - (2), d - (1), e - (1)

---

### Question 3

The following pseudocode is executed using the “Library” dataset. At the end of the execution, **A** captures the maximum number of pages of a book which is written in a language other than English. Choose the correct code fragment to complete the pseudocode.

`   xxxxxxxxxx  1  A = 0  2  while (Table 1 has more rows) {  3      Read the first row X in Table 1  4      *********************  5      * Fill the code *  6      *********************  7      Move X to Table 2  8  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Language == “English” and X.Pages > A){  2      A = X.Pages  3  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Language != “English” and X.Pages > A){  2      A = X.Pages  3  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Language != “English” and X.Pages < A){  2      A = X.Pages  3  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Language == “English” and X.Pages < A){  2      A = X.Pages  3  }       `

---

### Question 4

The following pseudocode is executed using the “Scores” table. At the end of the execution, **A** captures the second highest mark in Mathematics. Assume that **Max** holds the value of the highest mark in Mathematics. Choose the correct code fragment to complete the pseudocode.

`   xxxxxxxxxx  1  A = 0  2  while(Table 1 has more rows){  3      Read the first row X in Table 1  4      *********************  5      * Fill the code *  6      *********************  7      Move the row X to Table 2  8  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Mathematics > A){  2      A = X.Mathematics  3  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Mathematics > Max and X.Mathematics < A){  2      A = X.Mathematics  3  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Mathematics < Max and X.Mathematics > A){  2      A = X.Mathematics  3  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Mathematics < Max){  2      A = X.Mathematics  3  }       `

---

### Question 5

Let **X** be a row in the “Words” table. Let **isShortVerb** be a procedure to find whether the word in the row **X** is a verb with letter count at most five. Choose the correct code fragment to complete the pseudocode.

`   xxxxxxxxxx  1  Procedure isShortVerb(X)  2      *********************  3      * Fill the code *  4      *********************  5  End isShortVerb       `
- [ ] `   xxxxxxxxxx  1  if(X.PartOfSpeech == “Verb”){  2      return(True)  3  }  4  else{  5      return(False)  6  }       `
- [ ] `   xxxxxxxxxx  1  if(X.PartOfSpeech == “Verb” and X.LetterCount ≤ 5){  2      return(False)  3  }  4  else{  5      return(True)  6  }       `
- [ ] `   xxxxxxxxxx  1  if(X.PartOfSpeech == “Verb” or X.LetterCount ≤ 5){  2      return(True)  3  }  4  else{  5      return(False)  6  }       `
- [ ] `   xxxxxxxxxx  1  if(X.PartOfSpeech == “Verb” and X.LetterCount ≤ 5){  2      return(True)  3  }  4  else{  5      return(False)  6  }       `

---

### Question 6

The following pseudocode is executed using the “Words” table. What will **A** represent at the end of execution?

`   xxxxxxxxxx  1  A = 0  2  while(Table 1 has more rows){  3      Read the first row X in Table 1  4      i = 1, B = True  5      while(i ≤ X.LetterCount){  6          if(ith letter of X.Word is a vowel){  7              B = False  8          }  9          i = i + 1  10      }  11      if(B){  12          A = A + 1  13      }  14      Move X to Table 2  15  }       `
- [ ] Number of words with at most one vowel
- [ ] Number of words with at exactly one vowel
- [ ] Number of words without vowels
- [ ] Number of words with vowel count at most 2

---

### Question 7

The following pseudocode is executed using the “Library” dataset. At the end of the execution, **A** captures the number of books which are published after 2010 or have less than the average number of pages. Assume that the variable **Avg** holds the value of the average number of pages of the books in the table. The pseudocode may have mistakes. Identify all such mistakes (if any). It is a Multiple Select Question (MSQ).

`   xxxxxxxxxx  1  A = 0  2  while(Table 1 has more rows){  3      Read the first row X in Table 1  4      C = False  5      if(X.Year > 2010){  6          C = True  7      }  8      if(X.Pages > Avg){  9          C = True  10      }  11      if(C){  12          A = 1  13      }  14      Move X to Table 2  15  }       `
- [ ] Error in Line 5
- [ ] Error in Line 8
- [ ] Error in Line 9
- [ ] Error in Line 12
- [ ] No error

---

### Question 8

The following pseudocode is executed using the “Library” dataset. At the end of the execution, **A** is set to True if and only if there is a pair of books with same genre and same year of publication. Choose the correct code fragment to complete the pseudocode.

`   xxxxxxxxxx  1  A = False  2  while(Table 1 has more rows){  3      Read the first row X in Table 1  4      Move X to Table 2  5      while(Table 1 has more rows){  6          Read the first row Y in Table 1  7          Move Y to Table 3  8          *********************  9          * Fill the code *  10          *********************  11      }  12      Move all rows from Table 3 to Table 1  13  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Genre == Y.Genre or X.Year == Y.Year){  2      A = True  3  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Genre == Y.Genre and X.Year == Y.Year){  2      A = True  3  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Genre == Y.Genre or X.Year == Y.Year){  2      A = False  3  }       `
- [ ] `   xxxxxxxxxx  1  if(X.Genre == Y.Genre and X.Year == Y.Year){  2      A = False  3  }       `

---

### Question 9

The following pseudocode is executed using the “Library” table. What will the values of the variables **A** and **B** represent at the end of the execution?

`   xxxxxxxxxx  1  A = 0, B = 0  2  while(Table 1 has more rows){  3      Read the first row X in Table 1  4      if(X.Pages == A){  5          B = B + 1  6      }  7      if(X.Pages > A){  8          A = X.Pages  9          B = 1  10      }  11      Move X to Table 2  12  }       `
- [ ] **A** = Number of books with maximum number of pages  **B** = Maximum number of pages across all books
- [ ] **A** = Maximum number of pages across all books  **B** = Number of books with maximum number of pages
- [ ] **A** = Minimum number of pages across all books  **B** = It is always one
- [ ] **A** = Maximum number of pages across all books  **B** = It is always one

---

### Question 10

The following pseudocode is executed using the “Words” dataset. What will the value of **C** represent at the end of the execution?

`   xxxxxxxxxx  1  C = 0  2  while(Table 1 has more rows){  3      Read the first row X from Table 1  4      Move X to Table 2  5      if(X.Word ends with a full stop){  6          C = C + GetSomething(Table 2)  7          Clear all rows in Table 2  8      }  9  }  10  ​  11  Procedure GetSomething(Table 2)  12      A = 0  13      While(Table 2 has more rows){  14          Read the first row X in Table 2  15          Move X to Table 3  16          while(Table 2 has more rows){  17              Read the first row Y in Table 2  18              if(X.LetterCount != Y.LetterCount and X.PartOfSpeech == Y.PartOfSpeech){  19                  A = A + 1  20              }  21              Move Y to Table 4  22          }  23          Move all rows from Table 4 to Table 2  24      }  25      return (A)  26  End GetSomething       `
- [ ] Number of pairs of words with the same part of speech and letter count
- [ ] Number of pairs of words with the same part of speech and different letter count
- [ ] Number of pairs of words with the same part of speech and letter count, that occur in the same sentence
- [ ] Number of pairs of words with same part of speech and different letter count, that occur in the same sentence

---

### Question 11

Let **A** be an author who had written a book in the “Library” dataset and **B** be a positive integer value. What does the procedure DoSomething compute?

`   xxxxxxxxxx  1  Procedure DoSomething(A, B)  2      C = 1900, D = 2022  3      while(Table 1 has more rows){  4          Read the first row X in Table 1  5          if(X.Author == A){  6              if(X.Year > C){  7                  C = X.Year  8              }  9              if(X.Year < D){  10                  D = X.Year  11              }  12          }  13          Move X to Table 2  14      }  15      if(C − D ≥ B){  16          return(True)  17      }  18      else{  19          return(False)  20      }  21  End DoSomething       `
- [ ] Outputs “True” if and only if the second book of the author **A** was published at least **B** years after their first book was published
- [ ] Outputs “True” if and only if the last book of the author **A** was published at least **B** years after their first book was published
- [ ] Outputs “True” if and only if the last book of the author **A** was published at least **B** years after their second-last book was published
- [ ] Outputs “True” if and only if the last book of the author **A** was published at least **B** years before their first book was published

---

### Question 12

The following pseudocode is executed using the “Scores” dataset. At the end of the execution, **A** captures the number of female students who are above average in at least one subject. Assume that **M**, **P** and **C** hold the average marks of the subjects Mathematics, Physics and Chemistry respectively. The pseudocode may have mistakes. Identify all such mistakes (if any). It is a Multiple Select Question (MSQ).

`   xxxxxxxxxx  1  A = 0  2  while(Table 1 has more cards){  3      Read the first row X from Table 1  4      if(CheckSomething(X, M, P, C)){  5          A = 1  6      }  7      Move X to Table 2  8  }  9  Procedure CheckSomething(Y, C1, C2, C3)  10      if(Y.Gender == “F”){  11          if(Y.Mathematics > C1 and Y.Physics > C2 and Y.Chemistry > C3){  12              return (True)  13          }  14          else{  15              return(False)  16          }  17      }  18      else{  19          return(False)  20      }  21  End CheckSomething       `
- [ ] Error in Line 4
- [ ] Error in Line 5
- [ ] Error in Line 10
- [ ] Error in Line 11
- [ ] Multiple return(False) in procedure **CheckSomething**
- [ ] No error

---

### Question 13

The following pseudocode is executed using the “Words” table. At the end of the execution, **A** captures the number of sentences with at least two nouns that have at most 2 vowels. The pseudocode may have mistakes. Identify all such mistakes (if any). It is a Multiple Select Question (MSQ).

`   xxxxxxxxxx  1  A = 0, C = 0  2  while(Table 1 has more cards){  3      Read the first row X from Table 1  4      if(X.PartOfSpeech == “Noun” and CountVowels(X) ≤ 2){  5          C = C + 1  6      }  7      if(X.Word ends with a full stop){  8          if(C ≥ 2){  9              A = A + 1  10              C = 0  11          }  12      }  13      Move X to Table 2  14  }  15  Procedure CountVowels(Y)  16      i = 1  17      B = 0  18      while(i ≤ Y.LetterCount){  19          if(ith letter of Y.Word is a vowel){  20              B = B + 1  21              i = i + 1  22          }  23      }  24      return(B)  25  End CountVowel       `
- [ ] Line 5: Error in updating **C**
- [ ] Line 9: **A** is updated in wrong place
- [ ] Line 10: **C** is updated in wrong place
- [ ] Line 20: **B** is updated in wrong place
- [ ] Line 21: **i** is updated in wrong place
- [ ] Line 24: Return value is incorrect

---

### Question 14

The following pseudocode is executed using the “Scores” table. At the end of the execution, **C** captures the number of pairs of students who have the same date of birth, or the same City/Town but different gender. Choose the correct code fragment(s) to complete the pseudocode. It is a Multiple Select Question (MSQ).

`   xxxxxxxxxx  1  C = 0  2  while(Table 1 has more rows){  3      Read the first row X in Table 1  4      Move X to Table 2  5      while(Table 1 has more rows){  6          Read the first row Y in Table 1  7          Move Y to Table 3  8          *********************  9          * Fill the code *  10          *********************  11      }  12      Move all rows from Table 3 to Table 1  13  }       `
- [ ] `   xxxxxxxxxx  1  if(X.DateOfBirth == Y.DateOfBirth){  2      C = C + 1  3  }  4  if(X.Gender != Y.Gender and X.CityTown == Y.CityTown){  5      C = C + 1  6  }       `
- [ ] `   xxxxxxxxxx  1  if(X.DateOfBirth == Y.DateOfBirth){  2      C = C + 1  3  }  4  else{  5      if(X.Gender != Y.Gender and X.CityTown == Y.CityTown){  6          C = C + 1  7      }  8  }       `
- [ ] `   xxxxxxxxxx  1  if(X.DateOfBirth == Y.DateOfBirth){  2      if(X.Gender != Y.Gender and X.CityTown == Y.CityTown){  3          C = C + 1  4      }  5  }       `
- [ ] `   xxxxxxxxxx  1  if((X.DateOfBirth == Y.DateOfBirth) or (X.Gender != Y.Gender and X.CityTown == Y.CityTown)){  2      C = C + 1  3  }       `

---

