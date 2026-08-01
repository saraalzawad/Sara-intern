# Data Visualization Reflection

I learned that charts make data easy to understand. A line chart shows changes, a bar chart compares values, and a scatter plot shows if two things are connected. Seaborn helps make charts look better. Focus Bear can use charts to understand user data.

## Line Chart

```python
import matplotlib.pyplot as plt

plt.plot([1, 2, 3], [2, 4, 6])
plt.show()
```

Shows changes over time.

## Bar Chart

```python
import matplotlib.pyplot as plt

plt.bar(["A", "B", "C"], [3, 5, 2])
plt.show()
```

Compares values.

## Scatter Plot

```python
import matplotlib.pyplot as plt

plt.scatter([1, 2, 3], [2, 4, 6])
plt.show()
```

Shows the relationship between two values.

## Histogram

```python
import seaborn as sns

sns.histplot([2, 3, 3, 4, 5])
```

Shows how the data is spread.
