**Definition:** 
 A domain-specific language used for managing and manipulating relational databases.

A programming language used to create, interact with and request information from a database
used by most web applications
websites use images and menus for the SQL queries run 
retriever, insert, update and delete information in tables using [[Query]](-y)ies
[[SQLi (Structured Query Language Injection)]]
used to review [[log]]s
different versions can be accessed throughout [[Linux Commands]]
[[Syntax]]
Used for [[Filtering]]
[[Operator]]
Semi-colons should be placed at the end of the statement
\*\ -  Wild card meaning all
**SELECT** - indicates which columns to return (use commas to sperate each column)
**FROM** - indicates which table to query e.g. FROM customersTable
**ORDER BY** - sequences the records returned based on a specific column or columns. Can be ascending or descending order. e.g. ORDER BY city DESC (for descending)
**DESC** - used after the ordered column in ORDER BY for descending order (ascending by default)
If you order by several columns it will order by the left most column then it will order the results with the same leftmost column by the second left most column and so on e.g.
![[Pasted image 20231005153427.png]]

`sudo mysql organization` : if unintentionally exit data base by doing ctrl + c
ctrl + L to clear
WHERE - indicates the condition for a filter (put chosen data in quotes )
% - any other characters e.g. SELECT ... FROM ... WHERE direction LIKE 'East%' would return all rows with EASTsomething as their direction
Must use LIKE when using % wildcard
LIKE - Used with WHERE to search for a pattern in a column
_ - A wildcard similar to LIKE however it only substitutes for one other character whilst the % wildcard substitutes for any number of characters
![[Pasted image 20231005155515.png]]

Data Types:
String - Data consisting of an ordered sequence of characters (numbers letters or symbols)
Numeric - Data consisting of numbers
Date & Time - Data representing a date &or time
Operators:
= Equal to
\> Greater than
< Less than
<> Not Equal to 
!= Not Equal to
\>= Greater than or equal to
\< Less than or equal to 

BETWEEN - an inclusive operator that filters for numbers or dates within a range (Inclusive)
AND - Specifies that both conditions must be met simultaneously
e.g. BETWEEN '2018' AND '2020'                     (2018, 2019, 2020,)
quotation marks aren't used for numbers only for date & Time and strings
OR - specifies that either condition can be met
NOT - negates a condition 
TRUE (1) 
FALSE (0) 
e.g. WHERE NOT country = 'USA'
e.g. WHERE country != 'USA'
e.g. WHERE country <> 'USA'
Are all the same
`WHERE country NOT LIKE 'MEX%'` need to use NOT for % & _ wildcard (since using LIKE)

tableName.columnName
join foreign key onto primary key
e.g. 
`SELECT *`
`FROM employees`
`INNER JOIN machines ON employees.device_id = machines.device_id;`
(first/left table after FROM)
(second/right table after JOIN)

`INNER JOIN`: Returns rows matching on a specified column that exists in more than one table
![[Pasted image 20231008130824.png]]

empty records are indicated by NULL


Outer join types:
`LEFT JOIN`- Returns all of the records of the first table but only return rows of the second table that match on a specified column
![[Pasted image 20231008131106.png]]
`RIGHT JOIN` - Returns all of the records of the second table but only return rows of the first table that match on a specified column
![[Pasted image 20231008131116.png]]
`FULL OUTER JOIN` - Returns all records from all tables
![[Pasted image 20231008131127.png]]


aggregate functions: functions that perform a calculation over multiple data points and return the result of the calculation. 
`COUNT`- returns a single number that represents the number of rows returned from your query
`AVG` - returns a single number that represents the average of the numerical data in a column
`SUM` - returns a single number that represents the sum of the numerical data in a column

To use an aggregate function place the keyword for it after the SELECT keyword
E.G.
`SELECT COUNT(firstname)
`FROM customers;`
The result is a table with one column titled COUNT (firstname) and one row that indicates the count.
![[Pasted image 20231008132630.png]]
You can still add filters to your query e.g.
SELECT COUNT(firstname)
FROM customers
WHERE country = 'USA'