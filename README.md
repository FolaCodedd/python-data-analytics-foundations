# 📊 Machine Learning & Statistics Assignments
**Folayinka Olaofe** · Data Analytics Portfolio

A collection of Python/Jupyter notebooks completed as part of coursework in data analytics and applied statistics. Each notebook is self-contained and demonstrates a different skillset — from data wrangling with NumPy/Pandas, to exploratory data analysis and visualisation, to hypothesis testing.

---

## 📁 Notebooks

### Assignment 1 — Data Wrangling & Matrix Operations (`PROG50141`)
**Dataset:** Sales CSV (Kaggle)

Covers the fundamentals of working with structured data in Python:
- Loading CSV data into a Pandas DataFrame
- Selecting and operating on columns as NumPy arrays (vectors)
- Computing descriptive stats: mean, min, max; applying vectorized transformations
- Building and operating on NumPy matrices — shape, column-wise means, row-wise sums
- Matrix normalization (Min-Max), transposition, and scalar multiplication
- Data wrangling: dropping irrelevant columns, renaming for clarity, grouping by state, and filtering for loss-making transactions

---

### Assignment 2 — EDA, Visualisation & Sampling (`STAT53894`)
**Dataset:** World Happiness Report 2025 (`WHR25_Data_Figure_2.1v3.xlsx`)

End-to-end exploratory data analysis pipeline on global happiness data:
- Filtering data to a target year range (2020–2024)
- Missing value treatment: dropping rows with excessive nulls; median imputation via `sklearn` for isolated missing values
- Country name standardisation using a replacement dictionary
- Ranking the top 10 and bottom 10 happiest countries for the most recent year
- Manual region mapping to enable regional comparisons (mean & variance of Life Ladder scores between Western Europe and Sub-Saharan Africa)
- Histogram of happiness scores — identified left skew in the distribution
- Correlation heatmap across the six core happiness metrics (GDP, Social Support, Health, Freedom, Generosity, Corruption)
- Multivariate "Drivers of Happiness" scatter plot (Happiness Score vs. GDP, coloured by region)
- Identified and interpreted a regional paradox in the data

---

### Assignment 3 — Hypothesis Testing (`STAT53894`)
**Dataset:** `tips` (Seaborn built-in)

Applied the full 6-step hypothesis testing process across three statistical tests:

| Task | Test | Business Question | Result |
|------|------|-------------------|--------|
| 1 | Independent samples t-test | Do male customers tip significantly more than female? | No significant difference (p = 0.93) |
| 2 | One-Way ANOVA (F-test) | Does day of the week affect total bill amount? | Significant effect found (F = 2.77, p = 0.04) — weekends drive higher bills |
| 3 | Chi-square test of independence | Is smoking behaviour independent of dining time? | No relationship found (p = 0.48); confirmed via permutation resampling |

Each task includes justification for test selection, significance level setting (α = 0.05), interpretation, and a business recommendation.

---

## 🛠️ Tech Stack

| Library | Usage |
|---------|-------|
| `pandas` | Data loading, filtering, grouping, wrangling |
| `numpy` | Vectors, matrices, numerical operations |
| `matplotlib` | Histograms, custom plots |
| `seaborn` | Heatmaps, dataset loading |
| `scipy.stats` | t-test, ANOVA, chi-square |
| `statsmodels` | OLS regression, ANOVA table, Welch's t-test |
| `sklearn` | `SimpleImputer` for missing value handling |

---

## 🚀 Running the Notebooks

1. Clone this repo:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy statsmodels scikit-learn openpyxl
   ```

3. Launch Jupyter:
   ```bash
   jupyter notebook
   ```

4. Open any `.ipynb` file and run all cells. Note: Assignment 1 requires `Sales_csv.csv` and Assignment 2 requires `WHR25_Data_Figure_2.1v3.xlsx` to be present in the same directory.

---

## 👤 About

**Olaofe Folayinka Oluwatoyosi**  
Background in ERP systems development and business reporting. Currently expanding into data analytics and machine learning.

> These notebooks represent coursework completed as part of a data analytics program — individual assignments rather than end-to-end projects, each focused on a specific concept or technique.
