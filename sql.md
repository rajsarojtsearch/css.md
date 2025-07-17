A: SQL (Structured Query Language) is used to communicate with and manipulate databases.

2. Q: What are the different types of SQL commands?
   A: DDL (Data Definition Language), DML (Data Manipulation Language), DCL (Data Control Language), TCL (Transaction Control Language).

3. Q: What is the difference between DELETE and TRUNCATE?
   A: DELETE removes specific rows and can be rolled back, whereas TRUNCATE removes all rows and cannot be rolled back.

4. Q: What is a Primary Key?
   A: A unique identifier for a record in a table that cannot have NULL values.

5. Q: What is a Foreign Key?
   A: A column that establishes a relationship between two tables.

6. Q: What is an Index in SQL?
   A: A database object that improves the speed of queries on a table.

7. Q: What is the difference between UNIQUE and PRIMARY KEY constraints?
   A: UNIQUE allows NULL values, whereas PRIMARY KEY does not.

8. Q: What is a JOIN in SQL?
   A: A JOIN is used to combine rows from two or more tables based on a related column.

9. Q: Explain the types of JOINs in SQL.
   A: INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN, CROSS JOIN.

10. Q: What is a Subquery in SQL?
    A: A query within another query used to retrieve data.

11. Q: What is Normalization?
    A: The process of organizing data to reduce redundancy and improve efficiency.

12. Q: What are the different Normal Forms?
    A: 1NF, 2NF, 3NF, BCNF, 4NF, 5NF.

13. Q: What is Denormalization?
    A: The process of combining tables to improve read performance.

14. Q: What is ACID in SQL?
    A: Atomicity, Consistency, Isolation, Durability - properties of transactions.

15. Q: What is a View?
    A: A virtual table based on the result of a SQL query.

16. Q: What is the difference between WHERE and HAVING clauses?
    A: WHERE filters rows before grouping, HAVING filters groups after aggregation.

17. Q: What is a Stored Procedure?
    A: A set of SQL statements stored in the database for reuse.

18. Q: What is a Trigger in SQL?
    A: A stored procedure that automatically executes in response to certain events.

19. Q: What is a Cursor?
    A: A database object used to retrieve rows one by one from a result set.

20. Q: What is a Transaction in SQL?
    A: A sequence of operations performed as a single logical unit.

21. Q: What is the difference between UNION and UNION ALL?
    A: UNION removes duplicates, UNION ALL retains them.

22. Q: What is the difference between CHAR and VARCHAR?
    A: CHAR has a fixed length, VARCHAR has a variable length.

23. Q: What is the difference between RANK() and DENSE_RANK()?
    A: RANK() skips ranks after duplicates, while DENSE_RANK() does not.

24. Q: What is the COALESCE function?
    A: Returns the first non-null value in a list of expressions.

25. Q: What is the CASE statement in SQL?
    A: A conditional statement similar to IF-ELSE.

26. Q: What is the difference between a Clustered and Non-Clustered Index?
    A: Clustered indexes define physical storage order, non-clustered do not.

27. Q: What is the difference between a Cross Join and a Full Outer Join?
    A: Cross Join produces a Cartesian product, Full Outer Join combines matching and unmatched rows.

28. Q: What is the difference between GROUP BY and PARTITION BY?
    A: GROUP BY aggregates rows, PARTITION BY segments data without aggregating.

29. Q: What is the function of NOW() in SQL?
    A: Returns the current date and time.

30. Q: What are Aggregate Functions in SQL?
    A: Functions like SUM, COUNT, AVG, MAX, MIN used for calculations.

31. Q: What is the difference between BETWEEN and IN operators?
    A: BETWEEN specifies a range, IN specifies multiple discrete values.

32. Q: What is the use of the LIMIT clause?
    A: Restricts the number of returned records.

33. Q: What is a Recursive Query in SQL?
    A: A query that references itself using CTE (Common Table Expression).

34. Q: What is the difference between IN and EXISTS?
    A: IN checks for values in a list, EXISTS checks for row existence.

35. Q: What is the use of FETCH and OFFSET?
    A: Used for pagination in queries.

36. Q: What is the purpose of EXPLAIN in SQL?
    A: Used to analyze and optimize query execution plans.

37. Q: What are Window Functions in SQL?
    A: Functions that perform calculations across a subset of rows.

38. Q: What is the difference between MERGE and UPSERT?
    A: MERGE combines INSERT, UPDATE, DELETE in one query, UPSERT inserts if not exists, updates otherwise.

39. Q: What is Referential Integrity?
    A: Ensuring relationships between tables remain consistent.

40. Q: What is the difference between SERIALIZABLE and READ COMMITTED isolation levels?
    A: SERIALIZABLE ensures full isolation, READ COMMITTED allows reading committed data.

41. Q: What is a Deadlock in SQL?
    A: A situation where two transactions wait indefinitely for each other to release resources.

42. Q: What are Check Constraints?
    A: Constraints that enforce specific rules on column values.

43. Q: What is the ROW_NUMBER() function?
    A: Assigns a unique number to each row in a result set.

44. Q: What is the difference between LAG() and LEAD()?
    A: LAG() accesses previous row values, LEAD() accesses next row values.

45. Q: What is a Materialized View?
    A: A physical copy of query results stored for performance.

46. Q: What is the NVL function in SQL?
    A: Replaces NULL with a specified default value.

47. Q: What is an Auto-Increment column?
    A: A column where values are automatically generated.

48. Q: What is the difference between IFNULL() and ISNULL()?
    A: IFNULL() is used in MySQL, ISNULL() is used in SQL Server.

49. Q: What is the CASE WHEN statement?
    A: A conditional statement similar to an IF-ELSE structure.

50. Q: What is the difference between DELETE CASCADE and DELETE SET NULL?
    A: DELETE CASCADE deletes related records, DELETE SET NULL sets related columns to NULL.


Explanation of Different Normal Forms in Database Normalization:
Normalization is the process of organizing data in a database to reduce redundancy and improve data integrity. Below are the different Normal Forms (NF):

1NF (First Normal Form) - Atomicity
Rules:

Each column must have atomic (indivisible) values.
Each column must contain values of a single type.
Each row must have a unique identifier (Primary Key).
Example (Not in 1NF):

Student_ID	Name	Courses
1	Alice	Math, Science
2	Bob	English, History
Problem: "Courses" column contains multiple values.

1NF Conversion:

Student_ID	Name	Course
1	Alice	Math
1	Alice	Science
2	Bob	English
2	Bob	History
2NF (Second Normal Form) - No Partial Dependency
Rules:

Must be in 1NF.
All non-key attributes must be fully dependent on the entire Primary Key (not just part of it).
Example (Not in 2NF):

Student_ID	Course_ID	Student_Name	Course_Name
1	101	Alice	Math
1	102	Alice	Science
2	103	Bob	English
Problem: Student_Name depends only on Student_ID, and Course_Name depends only on Course_ID (Partial Dependency).

2NF Conversion:

Student Table:

Student_ID	Student_Name
1	Alice
2	Bob
Course Table:

Course_ID	Course_Name
101	Math
102	Science
103	English
Enrollment Table: (Mapping Table)

Student_ID	Course_ID
1	101
1	102
2	103
3NF (Third Normal Form) - No Transitive Dependency
Rules:

Must be in 2NF.
There should be no transitive dependency (non-key attribute should not depend on another non-key attribute).
Example (Not in 3NF):

Student_ID	Student_Name	Course_ID	Course_Name	Instructor	Instructor_Department
1	Alice	101	Math	Dr. Smith	Mathematics
2	Bob	102	Science	Dr. John	Physics
Problem: Instructor_Department depends on Instructor, which is not a primary key (transitive dependency).

3NF Conversion:

Instructor Table:

Instructor	Instructor_Department
Dr. Smith	Mathematics
Dr. John	Physics
Course Table:

Course_ID	Course_Name	Instructor
101	Math	Dr. Smith
102	Science	Dr. John
BCNF (Boyce-Codd Normal Form) - Advanced 3NF
Rules:

Must be in 3NF.
For every functional dependency (A → B), A must be a super key.
Example (Not in BCNF):

Teacher_ID	Subject	Department
1	Math	Science
2	Physics	Science
3	History	Arts
Problem: Department is functionally dependent on Subject, but Subject is not a super key.

BCNF Conversion:

Subject Table:

Subject	Department
Math	Science
Physics	Science
History	Arts
Teacher Table:

Teacher_ID	Subject
1	Math
2	Physics
3	History
4NF (Fourth Normal Form) - No Multi-Valued Dependencies
Rules:

Must be in BCNF.
A table should not contain multi-valued dependencies.
Example (Not in 4NF):

Student_ID	Course	Hobby
1	Math	Chess
1	Science	Chess
1	Math	Music
1	Science	Music
Problem: Course and Hobby are independent attributes but stored in the same table.

4NF Conversion:

Student_Course Table:

Student_ID	Course
1	Math
1	Science
Student_Hobby Table:

Student_ID	Hobby
1	Chess
1	Music
5NF (Fifth Normal Form) - No Join Dependency
Rules:

Must be in 4NF.
No join dependency, meaning the table should not split further without losing data.
Example (Not in 5NF):

Employee_ID	Project_ID	Location
1	P1	India
1	P2	USA
2	P1	India
2	P3	Germany
Problem: Employee, Project, and Location have independent relations but are combined.

5NF Conversion:

Employee_Project Table:

Employee_ID	Project_ID
1	P1
1	P2
2	P1
2	P3
Project_Location Table:

Project_ID	Location
P1	India
P2	USA
P3	Germany
Conclusion:
Normal Form	Main Rule
1NF	No duplicate columns, atomic values.
2NF	No partial dependencies on a composite key.
3NF	No transitive dependencies.
BCNF	Every determinant is a candidate key.
4NF	No multi-valued dependencies.
5NF	No join dependencies.
These normalization rules help create efficient, scalable, and easy-to-maintain databases.
