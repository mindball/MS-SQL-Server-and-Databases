# CRUD
```
OR slow queries: 
SELECT LastName FROM Employees WHERE NOT (ManagerID = 3 OR ManagerID = 4)
better way: 
SELECT LastName FROM Employees WHERE ManagerID <> 3 AND ManagerID <> 4
```

## Comparing with NULL
```
NULL is a special value that means missing value
Not the same as 0 or a blank space
```
### Checking for NULL values
```
SELECT LastName, ManagerId FROM Employees
WHERE ManagerId = NULL -> alwas false

SELECT LastName, ManagerId FROM Employees
WHERE ManagerId IS NULL ->right (IS NOT)
```

## Views
### Simplify complex queries
### Limit access to data for certain users

## Insert
### Inserting rows into existing table:
```
INSERT INTO Projects (Name, StartDate)
	SELECT Name + ' Restructuring', GETDATE()
	FROM Departments
```
### Using existing records to create a new table:
```
SELECT CustomerID, FirstName, Email, Phone
	INTO CustomerContacts
	FROM Customers
```

## Sequences
```
Sequences are special object in SQL Server
Similar to IDENTITY fields
Returns an incrementing value every time it’s used
```
