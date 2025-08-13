Here’s a clean and well-structured **README.md** for your Iris dataset exploration project:

---

````markdown
# 🌸 Iris Dataset Exploration & Visualization

This project explores and visualizes the **Iris dataset** using **Pandas**, **Seaborn**, and **Matplotlib**.  
It covers **basic dataset exploration**, **statistical summaries**, and **various visualizations** to understand the relationships between different flower measurements and species.

---

## 📂 Project Overview

The Iris dataset is a classic dataset in machine learning, containing 150 samples of iris flowers, each with:
- Sepal length
- Sepal width
- Petal length
- Petal width  
and the **species** (`setosa`, `versicolor`, `virginica`).

This notebook:
1. **Loads** the Iris dataset using Seaborn.
2. **Explores** its structure, columns, and statistical properties.
3. **Visualizes** relationships and distributions using:
   - Scatter plots
   - Histograms
   - Box plots

---

## 📦 Libraries Used

```python
import pandas as pd
import seaborn as sb
import matplotlib.pyplot as plt
````

---

## 🔍 Steps & Features

### 1. **Data Loading**

```python
dataset = sb.load_dataset('iris')
```

* Shape, columns, first 6 rows, and data info are printed.
* Descriptive statistics (`count`, `mean`, `std`, `min`, `25%`, `50%`, `75%`, `max`) are shown.

---

### 2. **Scatter Plots**

* **Petal Length vs Petal Width** (by species)
* **Sepal Length vs Sepal Width** (by species)
* **Sepal Length vs Petal Length** (by species)
* **Sepal Width vs Petal Width** (by species)

Example:

```python
sb.scatterplot(x='petal_length', y='petal_width', data=dataset, hue='species')
```

---

### 3. **Histograms**

Plots distribution of:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

Example:

```python
sb.histplot(data=dataset, x='sepal_length', bins=20)
```

---

### 4. **Box Plots**

Visualizes spread and outliers for:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

Example:

```python
sb.boxplot(data=dataset, y='sepal_length')
```

---

## 📊 Output Samples

### Scatter Plot Example:

![Scatter Plot](https://seaborn.pydata.org/_images/seaborn-scatterplot-1.png)

### Histogram Example:

![Histogram](https://seaborn.pydata.org/_images/seaborn-histplot-1.png)

---

## 🚀 How to Run

1. Install required libraries:

```bash
pip install pandas seaborn matplotlib
```

2. Run the Jupyter/Colab notebook:

```bash
jupyter notebook DHC_3135_Task_1.ipynb
```

or open in **Google Colab**.

---

## 📌 Notes

* This is a beginner-friendly dataset exploration example.
* Can be extended for **machine learning classification tasks**.

---


