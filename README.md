# IMPLENTATION-OF-AGGREGATION-FUNCTIONS

AIM:

To implement on aggregation functions, grouping and ordering commands to manipulate tables in a database.

PROCEDURE:

An aggregate function allows you to perform a calculation on a set of values to return a single scalar value. We often use aggregate functions with the GROUP BY and HAVING clauses of the SELECT statement.

The following are the most commonly used SQL aggregate functions:

AVG – calculates the average of a set of values.

COUNT – counts rows in a specified table or view.

MIN – gets the minimum value in a set of values.

MAX – gets the maximum value in a set of values.

SUM – calculates the sum of values.

The SQL GROUP BY clause is used in collaboration with the SELECT statement to arrange identical data into groups. This GROUP BY clause follows the WHERE clause in a

SELECT statement and precedes the ORDER BY clause.

Syntax:

SELECT column1, column2

FROM table_name

WHERE [ conditions ]

GROUP BY column1, column2

ORDER BY column1, column2

The ORDER BY keyword is used to sort the result-set in ascending or descending order.

The ORDER BY keyword sorts the records in ascending order by default. To sort the records in descending order, use the DESC keyword.

Syntax;

SELECT column1, column2, ...

FROM table_name

ORDER BY column1, column2, ... ASC|DESC;

COMMANDS:

Let’s consider an employee table. We will perform the calculations on this table by using aggregate functions.

SQL> select AVG(salary) from employee;

SQL> select MAX(salary) from employee;

SQL> select MIN (salary) from employee;

SQL>select SUM (salary) from employee where city=’Pune’;

SQL> select COUNT(Empid) from employee;

SQL> select COUNT(*) from employee;

SQL> SELECT NAME, SUM(SALARY) FROM CUSTOMERS

GROUP BY NAME;

SQL> SELECT * FROM CUSTOMERS

ORDER BY NAME, SALARY;

SQL> SELECT * FROM CUSTOMERS

ORDER BY NAME DESC;

RESULT:

Thus the aggregation functions, grouping and ordering commands to manipulate tables in a database has been implemented and executes successfully.
