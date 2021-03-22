Edit the query to find how many inmates provided last statements.

```SQL
SELECT COUNT(last_statement) FROM executions;
```

Verify that 0 and the empty string are not considered NULL.

```SQL
SELECT (0 IS NOT NULL) AND ('' IS NOT NULL) ;
```

Find the total number of executions in the dataset.

```SQL
SELECT COUNT(first_name) FROM executions;
```

Verify that COUNT(*) gives the same result as before.

```SQL
SELECT COUNT(*) FROM executions;
```

This query counts the number of Harris and Bexar county executions. Replace SUMs with COUNTs and edit the CASE WHEN blocks so the query still works.

```SQL

```

Find how many inmates were over the age of 50 at execution time.

```SQL

```

Find the number of inmates who have declined to give a last statement.

```SQL

```

Find the minimum, maximum and average age of inmates at the time of execution.

```SQL

```

Find the average length (based on character count) of last statements in the dataset.

```SQL

```

List all the counties in the dataset without duplication.


```SQL

```

Find the proportion of inmates with claims of innocence in their last statements.

```SQL

```
