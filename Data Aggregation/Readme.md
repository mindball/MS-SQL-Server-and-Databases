# Data Aggregation

## Grouping
```
Grouping allows receiving data into separate groups
based on a common property
```

## Aggregate Functions

## Having Clause
```
The HAVING clause is used to filter data based on
aggregate values

We cannot use it without grouping first
```
```
Aggregate functions (MIN, MAX, SUM etc.) are
executed only once

Unlike HAVING, WHERE filters rows before
aggregation
```

## Pivot Tables
```
You can use the PIVOT and UNPIVOT relational operators to
change a table-valued expression into another table
```
```
PIVOT rotates a table-valued expression by turning the unique
values from one column in the expression into multiple
columns in the output, and performs aggregations where they
are required on any remaining column values that are wanted
in the final output
```
```
UNPIVOT performs the opposite operation to PIVOT by rotating
columns of a table-valued expression into column values
```
### Summarizes data from another table

### Applies an aggregate operation

### Typically includes grouping of the data