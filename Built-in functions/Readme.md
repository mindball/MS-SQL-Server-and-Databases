# Built in functions
## Aggregate functions
```
Aggregate functions perform a calculation on a set of values and return a
single value. They are allowed in the select list or the HAVING clause of a
SELECT statement. You can use an aggregation in combination with the
GROUP BY clause to calculate the aggregation on categories of rows.
```
## Analytic functions
```
Analytic functions compute an aggregate value based on a group of rows.
However, unlike aggregate functions, analytic functions can return
multiple rows for each group. You can use analytic functions to compute
moving averages, running totals, percentages, or top-N results within a
group.
```
## Ranking functions
```
Ranking functions return a ranking value for each row in a partition. Depending on
the function that is used, some rows might receive the same value as other rows.
```
## Rowset functions
```
Rowset functions Return an object that can be used like table references in an SQL
statement.
```
## Scalar functions
```
Operate on a single value and then return a single value. Scalar functions can be used
wherever an expression is valid.
```
## Function Collation
```
Functions that take a character string input and return a character
string output use the collation of the input string for the output.

Functions that take non-character inputs and return a character
string use the default collation of the current database for the
output.

Functions that take multiple character string inputs and return a
character string use the rules of collation precedence to set the
collation of the output string. For more information, see Collation
Precedence (Transact-SQL).
https://docs.microsoft.com/en-us/sql/t-sql/statements/collation-precedence-transact-sql?view=sql-server-2017
```
## TRANSLATE functions
```
returns the string provided as a first argument
after some characters specified in the second argument are
translated into a destination set of characters specified in the
third argument
```
```MSSQL code
	TRANSLATE ( inputString, characters, translations)
	SELECT TRANSLATE('2*[3+4]/{7-2}', '[]{}', '()()’);
		// 2*(3+4)/(7-2)
```





