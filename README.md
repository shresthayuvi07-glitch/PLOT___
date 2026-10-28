# 📊 Python Data Visualization: Matplotlib, Seaborn & Subplots

## 📌 Project Overview

This repository contains my Python data visualization practice and learning projects using **Matplotlib, Seaborn, and Subplots**. It covers fundamental to intermediate visualization techniques used in data analysis, exploratory data analysis (EDA), and data storytelling.

The goal of this project is to develop practical skills in presenting data through clear, meaningful, and professional charts.

## 🎯 Objectives

- Learn to create different types of charts using Matplotlib.
- Visualize statistical relationships using Seaborn.
- Create multiple charts in a single figure using subplots.
- Customize chart titles, labels, legends, colors, and styles.
- Perform exploratory data analysis using visualizations.
- Improve data interpretation and analytical skills.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Matplotlib** — Data visualization and chart customization
- **Seaborn** — Statistical data visualization
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computing
- **Jupyter Notebook / Google Colab** — Coding and experimentation

## 📚 Topics Covered

### 1. Matplotlib

Matplotlib is a Python library used to create static, animated, and interactive visualizations.

Topics include:
- Line charts
- Bar charts and horizontal bar charts
- Pie charts and donut charts
- Histograms
- Scatter plots
- Box plots
- Figure and axes customization
- Titles, axis labels, legends, markers, and grids
- Colors, line styles, and chart formatting

### 2. Seaborn

Seaborn is a statistical visualization library built on Matplotlib. It helps create attractive charts and explore relationships between variables.

Topics include:
- Scatter plots
- Line plots
- Bar plots
- Histograms and KDE plots
- Box plots and violin plots
- Count plots
- Heatmaps and correlation matrices
- Pair plots
- Categorical data visualization
- Visual exploratory data analysis (EDA)

### 3. Subplots

Subplots allow multiple charts to be displayed within a single figure, making comparisons easier.

Topics include:
- `plt.subplot()`
- `plt.subplots()`
- Rows and columns of charts
- Accessing individual axes
- Different chart types in one figure
- Figure size and layout adjustment
- Shared axes
- Chart spacing and titles
- Comparing multiple variables side by side

## 💻 Installation

Install the required libraries using pip:

```bash
pip install matplotlib seaborn pandas numpy jupyter
```

Import the libraries into Python:

```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import numpy as np
```

## 📈 Example: Matplotlib Subplots

```python
import matplotlib.pyplot as plt

days = ["Mon", "Tue", "Wed", "Thu", "Fri"]
sales = [120, 150, 100, 180, 200]
expenses = [80, 90, 75, 110, 130]

fig, axes = plt.subplots(1, 2, figsize=(12, 5))

axes[0].plot(days, sales, marker="o")
axes[0].set_title("Daily Sales")
axes[0].set_xlabel("Day")
axes[0].set_ylabel("Sales")

axes[1].bar(days, expenses)
axes[1].set_title("Daily Expenses")
axes[1].set_xlabel("Day")
axes[1].set_ylabel("Expenses")

plt.tight_layout()
plt.show()
```

## 📊 Example: Seaborn Visualization

```python
import seaborn as sns
import matplotlib.pyplot as plt

tips = sns.load_dataset("tips")

sns.scatterplot(
    data=tips,
    x="total_bill",
    y="tip",
    hue="day"
)

plt.title("Total Bill vs Tip")
plt.show()
```

## 📁 Suggested Repository Structure

```text
Python-Data-Visualization/
│
├── Matplotlib/
│   ├── line_chart.ipynb
│   ├── bar_chart.ipynb
│   ├── pie_chart.ipynb
│   └── histogram.ipynb
│
├── Seaborn/
│   ├── scatter_plot.ipynb
│   ├── box_plot.ipynb
│   ├── heatmap.ipynb
│   └── pairplot.ipynb
│
├── Subplots/
│   ├── basic_subplots.ipynb
│   ├── multiple_charts.ipynb
│   └── subplot_comparison.ipynb
│
└── README.md
```

*Note: The folder and notebook names above are suggested examples. Adjust them to match the files in your repository.*

## 🚀 Learning Outcomes

After completing this project, I aim to be able to:

- Create and customize different chart types.
- Analyze trends, distributions, and relationships in datasets.
- Build multi-chart visualizations using subplots.
- Perform visual exploratory data analysis.
- Communicate analytical findings through data visualization.
- Prepare visualizations for data analyst portfolios and projects.

## 🔮 Future Improvements

- Practice with real-world datasets.
- Create correlation heatmaps and pair plots.
- Combine Matplotlib and Seaborn in one figure.
- Build complete exploratory data analysis projects.
- Apply visualization techniques to business and sales datasets.
- Develop portfolio-ready charts and dashboards.

## 👨‍💻 Author

**Yubaraj Shrestha**

This repository represents my ongoing journey in Python programming, data analysis, and data visualization.

## ⭐ Support

If you find this repository useful, consider giving it a star ⭐ on GitHub.
