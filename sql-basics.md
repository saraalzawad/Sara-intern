# SQL Basics Reflection

I learned that SQL is useful for getting and organizing data from a database. The `WHERE` statement filters the data, while `GROUP BY` groups similar data together. SQL is useful with Python because SQL gets the data, and Python can be used to analyze it and make charts. In Focus Bear, SQL can be used to check user activity and create simple reports.

## SQL Examples

### Show all users

```sql
SELECT * FROM users;
```

This query shows all rows and columns from the `users` table.

### Show only active users

```sql
SELECT * FROM users
WHERE status = 'active';
```

This query only shows users whose status is `active`.

### Sort users by hours

```sql
SELECT * FROM users
ORDER BY hours DESC;
```

This query sorts users from the highest number of hours to the lowest.

### Count users by country

```sql
SELECT country, COUNT(*)
FROM users
GROUP BY country;
```

This query counts how many users are in each country.
