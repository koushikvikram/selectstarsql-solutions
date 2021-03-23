This query pulls the execution counts per county.
```SQL
SELECT county, COUNT(*) AS county_executions
FROM executions
GROUP BY county;
```

Modify this query so there are up to two rows per county — one counting executions with a last statement and another without.
```SQL
SELECT
  county,
  last_statement IS NOT NULL AS last_statement_present,
  COUNT(*)
FROM executions
GROUP BY county, last_statement_present
```

Count the number of inmates aged 50 or older that were executed in each county.
```SQL
SELECT county, COUNT(*) 
FROM executions
WHERE ex_age >= 50
GROUP BY county;
```

List the counties in which more than 2 inmates aged 50 or older have been executed.
```SQL
SELECT county
FROM executions
WHERE ex_age>=50
GROUP BY county
HAVING COUNT(*)>2;
```
