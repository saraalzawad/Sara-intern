# Data Visualization Reflection

## Why is data visualization important in analytics?

Data visualization helps turn data into charts that are easier to understand. It makes it easier to find patterns, trends, and compare results. Charts also help people explain data more clearly than tables.

## What types of charts are most useful for different types of data?

- **Line chart** – Shows changes over time.
- **Bar chart** – Compares different categories.
- **Scatter plot** – Shows the relationship between two variables.
- **Histogram** – Shows how data is distributed.
- **Heatmap** – Shows relationships or correlations between different values.

## How does Seaborn's advanced visualizations compare to Matplotlib's basic charts?

Matplotlib is useful for creating basic charts and gives more control over customization. Seaborn is built on top of Matplotlib and makes it easier to create attractive charts with less code. It also provides advanced charts like heatmaps.

## How could Focus Bear use visualizations to improve product decision-making?

Focus Bear could use charts to track user activity, feature usage, and productivity trends. By looking at these visualizations, the team can understand user behaviour, identify problems, and decide which features should be improved.

---

# Line Chart

```python
import matplotlib.pyplot as plt

months = ["Jan", "Feb", "Mar", "Apr"]
sales = [10, 15, 20, 25]

plt.plot(months, sales, color="blue", marker="o")
plt.title("Monthly Sales")
plt.xlabel("Month")
plt.ylabel("Sales")
plt.grid(True)

plt.show()
```

**Purpose:** Shows how values change over time.

---

# Bar Chart

```python
import matplotlib.pyplot as plt

categories = ["A", "B", "C"]
values = [5, 8, 3]

plt.bar(categories, values, color="green")
plt.title("Category Comparison")
plt.xlabel("Category")
plt.ylabel("Value")

plt.show()
```

**Purpose:** Compares values between categories.

---

# Scatter Plot

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [2, 4, 5, 4, 6]

plt.scatter(x, y, color="red")
plt.title("Scatter Plot Example")
plt.xlabel("X Values")
plt.ylabel("Y Values")

plt.show()
```

**Purpose:** Shows the relationship between two variables.

---

# Histogram

```python
import seaborn as sns
import matplotlib.pyplot as plt

data = [2, 3, 3, 4, 4, 5, 5, 6, 7, 8]

sns.histplot(data, bins=5, color="skyblue")

plt.title("Histogram Example")
plt.xlabel("Values")
plt.ylabel("Frequency")

plt.show()
```

**Purpose:** Shows how the data is distributed.

---

# Heatmap

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

data = pd.DataFrame(
    [[1.0, 0.8, 0.5],
     [0.8, 1.0, 0.6],
     [0.5, 0.6, 1.0]],
    columns=["Feature A", "Feature B", "Feature C"],
    index=["Feature A", "Feature B", "Feature C"]
)

sns.heatmap(data, annot=True, cmap="Blues")

plt.title("Correlation Heatmap")

plt.show()
```

**Purpose:** Shows the correlation between different variables.

---

# What I Learned

In this task I learned how Matplotlib and Seaborn can be used to create different types of charts. I also learned that adding titles, labels, and colours makes charts easier to understand. Seaborn provides more advanced visualizations like heatmaps, while Matplotlib is useful for creating basic charts. Data visualization is an important part of data analysis because it helps people understand information and make better decisions.