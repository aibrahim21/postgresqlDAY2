# postgresqlDAY2
using views, inbexes ,sequences,data types, functions on a database 
1. Selecting and Joining Tables:
SELECT: Used to query and retrieve data from tables.

JOIN: Used to combine rows from two or more tables based on a related column.

INNER JOIN: Returns rows where there is a match in both tables.

LEFT JOIN (if used): Returns all rows from the left table, and matching rows from the right table.

2. String Functions:
POSITION() / STRPOS() (PostgreSQL): Used to find the position of a substring in a string. Returns 0 if not found.

INSTR() (MySQL, SQLite): Similar to STRPOS() but used in MySQL and SQLite to find the position of a substring.

CHARINDEX() (SQL Server): Another function similar to INSTR() and POSITION() for finding the position of a substring in SQL Server.

REPLACE(): Replaces occurrences of a substring in a string with another substring.

3. Aggregate Functions:
AVG(): Calculates the average value of a numeric column, such as calculating the average grade.

ROUND(): Rounds numeric values to a specified number of decimal places.

4. Date and Time Functions:
NOW(): Returns the current date and time.

AGE(): Calculates the age based on the difference between a date (like a birthdate) and the current date.

EXTRACT(): Extracts a part of a date (e.g., year, month, day).

TO_CHAR(): Used to format dates and times into a specific string format. For example, 'MM-DD-YYYY' to display the date as 05-01-2025.

5. Inserting Data:
INSERT INTO: Adds new rows of data to a table. We used this to insert exam results and dates into the exam and grades tables.

VALUES: Specifies the data to be inserted into the columns of a table.

6. Foreign Key Constraints and Error Handling:
Foreign Keys: Used to ensure data integrity by linking columns between different tables (e.g., linking exam_id in grades to exam).

Error Handling: We encountered foreign key constraint errors when trying to insert values that violated these relationships (e.g., attempting to insert an exam_id into grades that doesn't exist in the exam table).

7. Calculating Differences:
TIMESTAMPDIFF() (MySQL): Used to calculate the difference between two timestamps.

AGE() (PostgreSQL): Calculates the interval between two dates, such as calculating the difference in years between a person's birthdate and the current date.

CURRENT_DATE / NOW(): Used to get the current date and time, often used in calculations involving differences in dates.

8. Updating Data:
UPDATE: Used to modify existing data in a table.

SET: Specifies the column(s) to be updated and their new value(s).

WHERE: Filters the rows that need to be updated based on certain conditions.

9. Removing Columns:
ALTER TABLE: Used to modify the structure of a table, such as dropping a column.

10. Handling Nulls:
IS NULL / IS NOT NULL: Used to check for NULL values in a column. This is important when filtering data that may have missing values.
