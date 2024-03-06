# SQL Mastery Showcase

Welcome to SQL Mastery Showcase! 🚀 This repository is a collection of SQL programs demonstrating advanced concepts in database management. Each program is carefully crafted to showcase the power and versatility of SQL in solving real-world scenarios.

## Library Database 📚

### Aim
Unleash the potential of table creation and view concepts.

### Schema

#### **BOOK**
- Book_id
- Title
- Publisher_Name
- Pub_Year

#### **BOOK_AUTHORS**
- Book_id
- Author_Name

#### **PUBLISHER**
- Name
- Address
- Phone

#### **BOOK_COPIES**
- Book_id
- Programme_id
- No-of_Copies

#### **BOOK_LENDING**
- Book_id
- Programme_id
- Card_No
- Date_Out
- Due_Date

#### **LIBRARY_PROGRAMME**
- Programme_id
- Programme_Name
- Address

### SQL Queries

1. **Retrieve details of all books:** Uncover the magic - ID, title, publisher name, authors, and copies in each programme.
2. **Borrower insights:** Who borrowed more than 3 books from Jan 2017 to Jun 2017?
3. **Delete a book:** Clean up like a pro. Delete a book in BOOK table, updating related tables seamlessly.
4. **Year-wise partitioning:** Dive into the past. Partition the BOOK table based on the year of publication.
5. **Current availability view:** Create a view of all books and their available copies in the Library.

## Order Database 🛍️

### Aim
Explore constraints and master update operations.

### Schema

#### **SALESMAN**
- Salesman_id
- Name
- City
- Commission

#### **CUSTOMER**
- Customer_id
- Cust_Name
- City
- Grade
- Salesman_id

#### **ORDERS**
- Ord_No
- Purchase_Amt
- Ord_Date
- Customer_id
- Salesman_id

### SQL Queries

1. **Grade above average:** Count customers with grades above Bangalore’s average.
2. **Multitasking salesmen:** Identify salesmen with more than one customer.
3. **City connectivity:** List all salesmen indicating those with and without customers in their cities.
4. **Top order view:** Create a view identifying the salesman with the highest order of the day.
5. **Farewell to a salesman:** Delete the salesman with ID 1000, gracefully removing all associated orders.

## Movie Database 🎬

### Aim
Master the art of JOIN operations.

### Schema

#### **ACTOR**
- Act_id
- Act_Name
- Act_Gender

#### **DIRECTOR**
- Dir_id
- Dir_Name
- Dir_Phone

#### **MOVIES**
- Mov_id
- Mov_Title
- Mov_Year
- Mov_Lang
- Dir_id

#### **MOVIE_CAST**
- Act_id
- Mov_id
- Role

#### **RATING**
- Mov_id
- Rev_Stars

### SQL Queries

1. **Hitchcock's collection:** List titles of all movies directed by Alfred Hitchcock.
2. **Actor's encore:** Find movies where an actor appeared in two or more films.
3. **Time-traveling actors:** List actors who appeared in a movie before 2000 and after 2015.
4. **Star-studded stats:** Display movie titles, stars, and the highest stars received, sorted alphabetically.
5. **Spielberg's masterpiece:** Update ratings of all Steven Spielberg's movies to a stellar 5.

## College Database 🎓

### Aim
Introduce PLSQL concepts with table usage.

### Schema

#### **STUDENT**
- USN
- SName
- Address
- Phone
- Gender

#### **SEMSEC**
- SSID
- Sem
- Sec

#### **CLASS**
- USN
- SSID

#### **COURSE**
- Subcode
- Title
- Sem
- Credits

#### **IAMARKS**
- USN
- Subcode
- SSID
- Test1
- Test2
- Test3
- FinalIA

### SQL Queries

1. **Semester spotlight:** List student details in the fourth semester 'C' section.
2. **Gender census:** Compute the total number of male and female students in each semester and section.
3. **Personal view:** Create a view showcasing Test1 marks of student USN '1BI15CS101' across all courses.
4. **Final excellence:** Calculate and update the FinalIA (average of the best two test marks) for all students.
5. **Categorize brilliance:** Categorize 8th-semester A, B, and C section students based on FinalIA.

## Company Database 💼

### Aim
Navigate the core with nested and correlated nesting queries, plus EXISTS and NOT EXISTS keywords.

### Schema

#### **EMPLOYEE**
- SSN
- Name
- Address
- Sex
- Salary
- SuperSSN
- DNo

#### **DEPARTMENT**
- DNo
- DName
- MgrSSN
- MgrStartDate

#### **DLOCATION**
- DNo
- DLoc

#### **PROJECT**
- PNo
- PName
- PLocation
- DNo

#### **WORKS_ON**
- SSN
- PNo
- Hours

### SQL Queries

1. **Scott's projects:** List project numbers involving employee 'Scott' and the resulting salaries after a 10% raise.
2. **Departmental finance:** Find the sum, max, min, and average salaries of all 'Accounts' department employees.
3. **Project devotees:** Retrieve employees working on all projects controlled by department number 5 (use NOT EXISTS).
4. **High earners in demand:** For departments with more than five employees, find those earning more than Rs.6,00,000.

Feel free to explore, contribute, and level up your SQL skills with these real-world scenarios! 🔍✨
