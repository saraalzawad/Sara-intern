# Pandas Data Manipulation Reflection

I already use Pandas in my university assignments, so I am familiar with it. Pandas makes it easy to load, filter, and clean data. I can use it to organize information and understand the data better. In Focus Bear, Pandas can help analyze user activity.

## Load Data

```python
df = pd.read_csv("users.csv")
```

## Filter Data

```python
df[df["status"] == "active"]
```

## Group Data

```python
df.groupby("country").size()
```

## Clean Data

```python
df.fillna(0)
```
