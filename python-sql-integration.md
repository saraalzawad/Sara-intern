# Python SQL Integration

## Example Code

```python
import psycopg
import pandas as pd

# Connect to PostgreSQL
conn = psycopg.connect(
    host="localhost",
    dbname="my_database",
    user="my_user",
    password="my_password"
)

# Load data into a DataFrame
query = "SELECT id, name, age FROM users;"
df = pd.read_sql(query, conn)

print(df)

# Pandas transformations
df = df[df["age"] > 18]
df["age_group"] = df["age"].apply(lambda x: "Adult")

print(df)

conn.close()
```

## Example Output

```
   id   name   age
0   1   Sara   22
1   2   Ali    17
2   3   John   30
```

After filtering:

```
   id   name   age  age_group
0   1   Sara   22   Adult
2   3   John   30   Adult
```

## Reflection

### Why is it useful to query databases directly from Python instead of using a SQL client?

Using Python makes it easy to automate data collection and analysis without running SQL manually.

### How does psycopg differ from psycopg2?

`psycopg` is the newer version and supports modern Python features.

### How can Pandas help with post-query data transformation?

Pandas can filter, sort, clean, and analyse the data after it is loaded.

### How could this integration be used to generate automated reports for Focus Bear?

Python can automatically query the database, process the data with Pandas, and create reports without manual work.