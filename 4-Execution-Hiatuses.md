Look up the documentation to fix the query so that it returns the number of days between the dates.
```SQL
SELECT JULIANDAY('1993-08-10') - JULIANDAY('1989-07-07') AS day_difference
```

Write a query to produce the previous table.
Remember to use aliases to form the column names(ex_number, last_ex_date). Hint: Instead of shifting dates back, you could shift ex_number forward!
```SQL
SELECT ex_number+1 AS ex_number, 
       ex_date AS last_ex_date 
FROM executions
WHERE ex_number<553;
```

