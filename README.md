# Exploratory Data Analysis (EDA) on the Iris Dataset

**Intern:** Rathod Harshvardhansinh
**Internship:** VEDA Technology, Data Analytics Track
**Task:** Level 1, Day 2: Exploratory Data Analysis (EDA)

## About the Project
This project explores the classic Iris dataset (150 flowers, 3 species, 4 measurements in cm) to find patterns, relationships, outliers and trends before drawing any conclusions. The goal was to build the habit of questioning data visually and statistically.

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- scikit-learn (only to load the dataset)

## Files in this Repository
| File | Description |
|------|-------------|
| `EDA_Iris_Analysis.ipynb` | Main Jupyter notebook with code, outputs, visualizations and written observations |

## What the Notebook Covers
1. Data quality check (missing values, duplicates, class balance)
2. Summary statistics (overall and per species)
3. Distributions using histograms and violin plots
4. Outlier detection using boxplots and the 1.5 x IQR rule
5. Correlation heatmap
6. Scatter plots showing relationships between features
7. Per-species regression lines to compare with the overall correlation
8. Top 3 insights and limitations

The notebook has **7 visualizations**, and each one has a written observation.

## Top 3 Insights
1. **Petal measurements separate the species best.** Setosa can be separated perfectly with a single cut-off (petal length under about 2 cm), while sepal measurements overlap too much.
2. **Pooled statistics can mislead.** Sepal length and width look uncorrelated overall (-0.12), but are positively correlated inside every species (0.46 to 0.74).
3. **The data is clean and the outliers are natural.** There are no missing values, the classes are balanced (50 each), and the only outliers (four sepal width values) are plausible measurements, so they were kept. Petal length and petal width are 0.96 correlated.

## How to Run
1. Open `EDA_Iris_Analysis.ipynb` in Jupyter Notebook or Google Colab.
2. Run all cells (**Runtime > Run all** in Colab).
3. Required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`.

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Limitations
- The dataset has only 150 rows, so patterns are indicative rather than conclusive.
- Iris has no date column, so a trend-over-time chart does not apply here.
- Measurements are rounded to 0.1 cm, which explains the one duplicate row.

## Author
Rathod Harshvardhansinh
