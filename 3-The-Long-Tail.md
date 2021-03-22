This query pulls the execution counts per county.
```SQL
SELECT county, COUNT(*) AS county_executions
FROM executions
GROUP BY county;
```

Modify this query so there are up to two rows per county — one counting executions with a last statement and another without.
```SQL

```

Count the number of inmates aged 50 or older that were executed in each county.
```SQL
SELECT county, COUNT(*) 
FROM executions
WHERE ex_age >= 50
GROUP BY county;
```
