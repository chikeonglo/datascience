<a href="../1. Fundamentals">Back to Fundamentals</a>

# SQL
***Resources:***
* <a href="https://sqlzoo.net/">SQLZOO</a>
* <a href="https://www.khanacademy.org/computing/computer-programming">Khan Academy - Computer Programming (Intro to SQL)</a>
* <a href="https://www.codecademy.com/learn/learn-sql">Code Academy - Learn SQL</a>

**Note:** these are only some of the resources, there are plenty of free resources online

## CRUD
This is the most important concept we need to know when dealing with databases. The main purpose of using SQL is to perform these function, which are
* Create
* Read
* Update
* Delete

This applies at both the table and the row level, therefore you need to know how to perform all 4 of these functions at both levels.  
You will likely be most familiar with the `read` functions, and the remainding sections will cover it in more detail. 

## Aggregation
Suppose you want to compute a single value from a set of inputs, here is how you can do it
```
SELECT FUNC(...) FROM table;
```
* `COUNT()`
* `MAX()`
* `MIN()`
* `AVG()`

Helper functions 
* `GROUP BY ...` - obtain a representative value for each unique group
* `ROUND()` 

## Multiple Tables
What is a relational database? Where the tables are linked together.  
How to link tables together? Using keys.  
Why do we link tables together? We can write queries that combine data from multiple tables 

### Linking tables
***Primary Key*** - unique identifier for each row in a table

***Foreign Key*** - contains the primay key of another table
* Just like any other columns
* do not need to be unique
* can be NULL

### Joins
* Cross Join - all rows combinations from 2 tables
* Inner Join - returns all rows where both key exists
* Outer Join (left / right)- return every row from one specified table, additional columns based on 2nd table tacked on

## Advanced
***Subqueries*** - nesting one query within another query
* Non-correlated - subquery independent of outer query
* Correlated - cannot be run independently of outer query
  * Order of operations: Row processed in outer query :rightarrow: subquery executed for that particular row

***Set Operations***
* `UNION` - distinct values from both tables
* `INTERSECT` - only common values from both tables
* `EXCEPT` - values in table 1 that isn't in table 2

***Conditional Aggregates*** - aggregate based on given conditions

***Manipulating Dates / Numbers / String***
* increment date/time
* summing / rounding / casting numbers
* concatenating / replacing strings

***Windows (running / rolling)*** - how values changes over time