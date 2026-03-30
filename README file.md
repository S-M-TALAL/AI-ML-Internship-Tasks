# AI-ML-Internship-Tasks
Exploratory Data Analysis on the Iris dataset with visualizations — AI/ML Engineering Internship Task 1
# 🌸 AI/ML Engineering Internship — Task 1: Iris Dataset Exploration & Visualization

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Task Objective

The goal of this task is to perform **Exploratory Data Analysis (EDA)** on the classic Iris dataset using Python. This includes:

- Loading and inspecting the dataset
- Identifying data distributions, correlations, and class separability
- Detecting outliers through visual analysis
- Generating and saving publication-quality visualizations

---

## 📂 Dataset Used

| Property        | Details                              |
|-----------------|--------------------------------------|
| **Name**        | Iris Dataset                         |
| **Source**      | Seaborn built-in (`sns.load_dataset('iris')`) |
| **Samples**     | 150 rows                             |
| **Features**    | 4 numerical + 1 categorical          |
| **Target**      | `species` (Setosa, Versicolor, Virginica) |
| **Missing Values** | None — clean dataset              |
| **Class Balance** | 50 samples per species (balanced) |

**Feature columns:** `sepal_length`, `sepal_width`, `petal_length`, `petal_width`

---

## 🤖 Models / Techniques Applied

> This task focuses on **data exploration and visualization** — no classification model is trained yet.

| Technique               | Purpose                                      |
|------------------------|----------------------------------------------|
| Descriptive Statistics  | Mean, std, min/max per feature               |
| Pairplot (Seaborn)      | Visualize pairwise feature relationships     |
| Scatter Plots           | Feature-vs-feature comparison by species     |
| Histograms + KDE        | Distribution shape per species               |
| Box Plots + Strip Plots | Outlier detection per feature per species    |

---

## 📊 Key Results & Findings

### 1. Dataset Overview
- 150 samples, 4 numerical features, 1 categorical target (`species`)
- Perfectly balanced classes (50 samples per species)
- No missing values — no preprocessing required

### 2. Feature Relationships
- **Petal length ↔ Petal width**: Strong positive correlation (~0.96) — best pair for species identification
- **Sepal length ↔ Petal length**: Moderate positive correlation (~0.87)
- **Sepal width ↔ Petal length**: Weak negative correlation (~−0.43)

### 3. Class Separability
- **Setosa** is clearly linearly separable from the other two species across all features
- **Versicolor** and **Virginica** show some overlap, especially in sepal measurements

### 4. Outliers
- A few outliers detected in `sepal_width` for Versicolor and Virginica
- Overall, the dataset is well-behaved with minimal noise

### 5. Best Features for Classification
Petal dimensions (`petal_length`, `petal_width`) provide the clearest separation between all three species and would be the most informative features for a classifier.

---

## 🗂️ Repository Structure

```
📦 ai-ml-internship-tasks/
├── 📓 AI_ML_Engineering_Internship_Tasks_1.ipynb   # Main notebook
├── 📄 README.md                                     # This file
└── 📁 output/
    ├── iris_pairplot.png       # Pairwise scatter plot matrix
    ├── iris_scatterplot.png    # Individual scatter plots (4 combinations)
    ├── iris_histogram.png      # Feature distributions by species
    └── iris_BoxPlot.png        # Outlier detection via box plots
```

---

## 🛠️ Libraries Used

```python
pandas        # Data loading and manipulation
numpy         # Numerical operations
matplotlib    # Base plotting
seaborn       # Statistical visualizations
os            # File/directory management
```

---

## ▶️ How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/S-M-TALAL/ai-ml-internship-tasks.git
   cd ai-ml-internship-tasks
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

4. Open `AI_ML_Engineering_Internship_Tasks_1.ipynb` and click **Run All**

> All output visualizations will be saved to the `output/` folder automatically.


