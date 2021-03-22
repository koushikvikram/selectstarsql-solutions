This query pulls the execution counts per county.
```SQL
SELECT county, COUNT(*) AS county_executions
FROM executions
GROUP BY county;
```

Modify this query so there are up to two rows per county — one counting executions with a last statement and another without.
```SQL

```
