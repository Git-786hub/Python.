# 🐍 Basic Python - Step by Step 

## Introduction

Python is a simple, powerful, and beginner-friendly programming language. This repository contains basic Python concepts explained step by step with examples.

## Prerequisites

* Install Python 3.12
* Verify installation:

```bash
python --version
```

## Step 1: Print Output

```python
print("Hello, World!")
```

**Output:**

```text
Hello, World!
```

## Step 2: Variables

```python
name = "Vishal"
age = 25

print(name)
print(age)
```

## Step 3: Data Types

```python
name = "Python"      # String
age = 25             # Integer
height = 5.8         # Float
is_student = True    # Boolean

print(type(name))
print(type(age))
print(type(height))
print(type(is_student))
```

## Step 4: User Input

```python
name = input("Enter your name: ")
print("Welcome", name)
```

## Step 5: Operators

```python
a = 10
b = 5

print(a + b)  # Addition
print(a - b)  # Subtraction
print(a * b)  # Multiplication
print(a / b)  # Division
```

## Step 6: Conditional Statements

```python
age = 18

if age >= 18:
    print("Eligible to vote")
else:
    print("Not eligible")
```

## Step 7: Loops

### For Loop

```python
for i in range(1, 6):
    print(i)
```

### While Loop

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

## Step 8: Functions

```python
def greet(name):
    return f"Hello, {name}"

print(greet("Vishal"))
```

## Step 9: Lists

```python
fruits = ["Apple", "Banana", "Mango"]

for fruit in fruits:
    print(fruit)
```

## Step 10: Dictionaries

```python
student = {
    "name": "Vishal",
    "age": 25
}

print(student["name"])
```

## Step 11: File Handling

```python
with open("sample.txt", "w") as file:
    file.write("Hello Python")
```

## Step 12: Exception Handling

```python
try:
    num = int(input("Enter a number: "))
    print(num)
except ValueError:
    print("Invalid input")
```

## Step 13: Object-Oriented Programming

```python
class Student:
    def __init__(self, name):
        self.name = name

    def display(self):
        print(self.name)

s1 = Student("Vishal")
s1.display()
```

## Step 14: Modules

```python
import math

print(math.sqrt(25))
```

## Learning Path

1. Print Statements
2. Variables & Data Types
3. Operators
4. Input & Output
5. Conditions
6. Loops
7. Functions
8. Lists & Dictionaries
9. File Handling
10. Exception Handling
11. OOP
12. Modules
Happy Coding! 🚀

# 🔢 NumPy Step-by-Step 

## Introduction

NumPy (Numerical Python) is the fundamental library for numerical computing in Python. It provides support for large multidimensional arrays, matrices, and high-level mathematical functions.

## What You Will Learn

* Installing NumPy
* Creating Arrays
* Array Operations
* Indexing & Slicing
* Reshaping Arrays
* Mathematical Functions
* Statistics
* Linear Algebra
* Random Numbers

---

# Step 1: Install NumPy

```bash
pip install numpy
```

Verify installation:

```python
import numpy as np

print(np.__version__)
```

---

# Step 2: Import NumPy

```python
import numpy as np
```

Conventionally, NumPy is imported as `np`.

---

# Step 3: Create Arrays

### 1D Array

```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])
print(arr)
```

Output:

```text
[1 2 3 4 5]
```

### 2D Array

```python
arr = np.array([[1, 2, 3],
                [4, 5, 6]])

print(arr)
```

---

# Step 4: Check Array Properties

```python
arr = np.array([[1,2,3],[4,5,6]])

print(arr.shape)
print(arr.ndim)
print(arr.size)
print(arr.dtype)
```

Output:

```text
(2, 3)
2
6
int64
```

---

# Step 5: Special Arrays

### Zeros

```python
np.zeros((3,3))
```

### Ones

```python
np.ones((2,4))
```

### Identity Matrix

```python
np.eye(3)
```

### Range

```python
np.arange(1,11)
```

### Evenly Spaced Values

```python
np.linspace(0,10,5)
```

---

# Step 6: Indexing and Slicing

```python
arr = np.array([10,20,30,40,50])

print(arr[0])
print(arr[-1])
```

### Slice

```python
print(arr[1:4])
```

Output:

```text
[20 30 40]
```

---

# Step 7: Array Operations

```python
a = np.array([1,2,3])
b = np.array([4,5,6])

print(a + b)
print(a - b)
print(a * b)
print(a / b)
```

Output:

```text
[5 7 9]
[-3 -3 -3]
[4 10 18]
[0.25 0.4 0.5]
```

---

# Step 8: Broadcasting

```python
arr = np.array([1,2,3])

print(arr + 10)
```

Output:

```text
[11 12 13]
```

---

# Step 9: Reshaping Arrays

```python
arr = np.arange(1,13)

new_arr = arr.reshape(3,4)

print(new_arr)
```

Output:

```text
[[ 1  2  3  4]
 [ 5  6  7  8]
 [ 9 10 11 12]]
```

---

# Step 10: Mathematical Functions

```python
arr = np.array([1,4,9,16])

print(np.sqrt(arr))
```

```python
print(np.sin(arr))
print(np.cos(arr))
print(np.log(arr))
```

---

# Step 11: Statistical Functions

```python
arr = np.array([10,20,30,40,50])

print(np.mean(arr))
print(np.median(arr))
print(np.std(arr))
print(np.max(arr))
print(np.min(arr))
print(np.sum(arr))
```

---

# Step 12: Sorting Arrays

```python
arr = np.array([5,2,8,1,9])

print(np.sort(arr))
```

Output:

```text
[1 2 5 8 9]
```

---

# Step 13: Filtering Arrays

```python
arr = np.array([10,20,30,40,50])

print(arr[arr > 25])
```

Output:

```text
[30 40 50]
```

---

# Step 14: Random Numbers

```python
np.random.rand(3)
```

```python
np.random.randint(1,100,5)
```

```python
np.random.seed(42)
```

---

# Step 15: Matrix Operations

```python
A = np.array([[1,2],
              [3,4]])

B = np.array([[5,6],
              [7,8]])

print(np.dot(A,B))
```

Output:

```text
[[19 22]
 [43 50]]
```

---

# Step 16: Linear Algebra

### Determinant

```python
np.linalg.det(A)
```

### Inverse

```python
np.linalg.inv(A)
```

### Eigenvalues

```python
np.linalg.eig(A)
```

---

# Step 17: Useful NumPy Functions

```python
np.unique([1,2,2,3,3,3])
```

```python
np.concatenate((a,b))
```

```python
np.vstack((a,b))
```

```python
np.hstack((a,b))
```

---

# Real-World Example

```python
import numpy as np

marks = np.array([78,85,92,67,88])

print("Average:", np.mean(marks))
print("Highest:", np.max(marks))
print("Lowest:", np.min(marks))
```

Output:

```text
Average: 82.0
Highest: 92
Lowest: 67
```

---


# Learning Roadmap

1. Arrays
2. Indexing & Slicing
3. Array Operations
4. Broadcasting
5. Reshaping
6. Mathematical Functions
7. Statistics
8. Random Numbers
9. Matrix Operations
10. Linear Algebra

---

# Why Learn NumPy?

✅ Faster than Python Lists
✅ Foundation for Pandas
✅ Essential for Machine Learning
✅ Used in Data Science and AI
✅ Efficient Memory Management

---
# 🐼 Pandas Step-by-Step 

## Introduction

Pandas is an open-source Python library used for data manipulation, analysis, and cleaning. It provides powerful data structures like **Series** and **DataFrame** that make working with structured data easy and efficient.

## What You Will Learn

* Installing Pandas
* Series
* DataFrames
* Reading & Writing Files
* Data Selection
* Filtering Data
* Handling Missing Values
* Grouping Data
* Merging DataFrames
* Data Analysis

---

# Step 1: Install Pandas

```bash
pip install pandas
```

Verify installation:

```python
import pandas as pd

print(pd.__version__)
```

---

# Step 2: Import Pandas

```python
import pandas as pd
```

Pandas is conventionally imported as `pd`.

---

# Step 3: Create a Series

A Series is a one-dimensional labeled array.

```python
import pandas as pd

data = pd.Series([10, 20, 30, 40, 50])

print(data)
```

Output:

```text
0    10
1    20
2    30
3    40
4    50
dtype: int64
```

---

# Step 4: Create a DataFrame

A DataFrame is a two-dimensional table.

```python
data = {
    "Name": ["Vishal", "Rahul", "Priya"],
    "Age": [22, 24, 21],
    "City": ["Pune", "Mumbai", "Delhi"]
}

df = pd.DataFrame(data)

print(df)
```

Output:

```text
     Name  Age    City
0  Vishal   22    Pune
1   Rahul   24  Mumbai
2   Priya   21   Delhi
```

---

# Step 5: View Data

```python
print(df.head())
```

First 5 rows:

```python
print(df.tail())
```

Last 5 rows:

```python
print(df.info())
```

Data information:

```python
print(df.describe())
```

Statistical summary:

---

# Step 6: Select Columns

```python
print(df["Name"])
```

Multiple columns:

```python
print(df[["Name", "Age"]])
```

---

# Step 7: Select Rows

Using `loc`

```python
print(df.loc[0])
```

Using `iloc`

```python
print(df.iloc[1])
```

---

# Step 8: Filtering Data

```python
print(df[df["Age"] > 22])
```

Output:

```text
    Name  Age    City
1  Rahul   24  Mumbai
```

Multiple conditions:

```python
print(df[(df["Age"] > 21) & (df["City"] == "Mumbai")])
```

---

# Step 9: Add New Column

```python
df["Salary"] = [30000, 45000, 35000]

print(df)
```

---

# Step 10: Update Values

```python
df.loc[0, "Age"] = 23
```

---

# Step 11: Delete Columns

```python
df.drop("Salary", axis=1, inplace=True)
```

Delete rows:

```python
df.drop(0, axis=0, inplace=True)
```

---

# Step 12: Handle Missing Values

Create missing values:

```python
import numpy as np

df["Salary"] = [30000, np.nan, 35000]
```

Check missing values:

```python
print(df.isnull())
```

Count missing values:

```python
print(df.isnull().sum())
```

Fill missing values:

```python
df["Salary"].fillna(df["Salary"].mean(), inplace=True)
```

Remove missing values:

```python
df.dropna(inplace=True)
```

---

# Step 13: Sorting Data

Sort by age:

```python
df.sort_values(by="Age")
```

Descending order:

```python
df.sort_values(by="Age", ascending=False)
```

---

# Step 14: Group By

```python
data = {
    "Department": ["IT", "HR", "IT", "HR"],
    "Salary": [50000, 40000, 60000, 45000]
}

df = pd.DataFrame(data)

print(df.groupby("Department")["Salary"].mean())
```

Output:

```text
Department
HR    42500
IT    55000
```

---

# Step 15: Read CSV File

```python
df = pd.read_csv("data.csv")

print(df.head())
```

---

# Step 16: Write CSV File

```python
df.to_csv("output.csv", index=False)
```

---

# Step 17: Read Excel File

```python
df = pd.read_excel("data.xlsx")
```

---

# Step 18: Write Excel File

```python
df.to_excel("output.xlsx", index=False)
```

---

# Step 19: Merge DataFrames

```python
df1 = pd.DataFrame({
    "ID": [1, 2, 3],
    "Name": ["A", "B", "C"]
})

df2 = pd.DataFrame({
    "ID": [1, 2, 3],
    "Salary": [30000, 40000, 50000]
})

merged = pd.merge(df1, df2, on="ID")

print(merged)
```

---

# Step 20: Pivot Table

```python
pivot = df.pivot_table(
    values="Salary",
    index="Department",
    aggfunc="mean"
)

print(pivot)
```

---

# Step 21: Real-World Example

Student Marks Analysis

```python
import pandas as pd

data = {
    "Student": ["A", "B", "C", "D"],
    "Marks": [85, 92, 78, 88]
}

df = pd.DataFrame(data)

print("Average Marks:", df["Marks"].mean())
print("Highest Marks:", df["Marks"].max())
print("Lowest Marks:", df["Marks"].min())
```

Output:

```text
Average Marks: 85.75
Highest Marks: 92
Lowest Marks: 78
```

---

# Learning Roadmap

1. Series
2. DataFrames
3. Data Selection
4. Filtering
5. Missing Values
6. Sorting
7. GroupBy
8. File Handling
9. Merging
10. Pivot Tables
11. Data Analysis

---

# Why Learn Pandas?

✅ Easy Data Cleaning
✅ Powerful Data Analysis
✅ Works with CSV, Excel, SQL
✅ Essential for Data Science
✅ Used in Machine Learning Pipelines
✅ Industry Standard Library

---

# Pandas + NumPy + Matplotlib Roadmap

```text
Python Basics
      ↓
NumPy
      ↓
Pandas
      ↓
Matplotlib
      ↓
Data Analysis
      ↓
Machine Learning
```
---

# 📊 Data Visualization with Python

## Introduction

Data Visualization helps transform data into charts and graphs for better understanding and decision-making.

### Libraries Used

* Matplotlib
* Seaborn
* Pandas

---

## Step 1: Install Libraries

```bash
pip install matplotlib seaborn pandas
```

---

## Step 2: Import Libraries

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

---

## Step 3: Create Sample Data

```python
data = {
    "Month": ["Jan", "Feb", "Mar", "Apr"],
    "Sales": [100, 150, 200, 180]
}

df = pd.DataFrame(data)
```

---

## Step 4: Line Chart

```python
plt.plot(df["Month"], df["Sales"])
plt.title("Monthly Sales")
plt.show()
```

---

## Step 5: Bar Chart

```python
plt.bar(df["Month"], df["Sales"])
plt.title("Sales by Month")
plt.show()
```

---

## Step 6: Pie Chart

```python
plt.pie(df["Sales"], labels=df["Month"], autopct="%1.1f%%")
plt.show()
```

---

## Step 7: Histogram

```python
plt.hist(df["Sales"])
plt.show()
```

---

## Step 8: Scatter Plot

```python
plt.scatter(df["Month"], df["Sales"])
plt.show()
```

---

## Step 9: Seaborn Bar Plot

```python
sns.barplot(x="Month", y="Sales", data=df)
plt.show()
```

---

## Step 10: Seaborn Heatmap

```python
corr = df.corr(numeric_only=True)

sns.heatmap(corr, annot=True)
plt.show()
```

---

## Mini Project

```python
import pandas as pd
import matplotlib.pyplot as plt

sales = [120, 180, 150, 220, 250]

plt.plot(sales, marker="o")
plt.title("Sales Trend")
plt.xlabel("Month")
plt.ylabel("Sales")
plt.show()
```

---

## Learning Roadmap

```text
Python Basics
      ↓
NumPy
      ↓
Pandas
      ↓
Matplotlib
      ↓
Seaborn
      ↓
Data Visualization
      ↓
Machine Learning
```

---

## Why Learn Data Visualization?

✅ Understand data quickly
✅ Identify trends and patterns
✅ Create dashboards and reports
✅ Essential for Data Science & Analytics

---



