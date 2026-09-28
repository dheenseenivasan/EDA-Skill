# Superstore Dataset Analysis

## Project Overview

This project analyzes a sample **Superstore dataset** using Python. The analysis is implemented in a Jupyter Notebook and focuses on sales, profit, discount, category-level performance, and correlations between numerical variables.

## Objective

The objective of this project is to explore the Superstore dataset and identify basic business insights using data analysis and visualization techniques.

## Dataset

The project uses `superstore_raw.csv`.

- **Rows:** 100
- **Columns:** 21
- **Country represented:** United States
- **Main business fields:** Category, Sub-Category, Sales, Quantity, Discount, Profit, Region, Segment, etc.

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## Project Files

```text
Superstore-Sales-Analysis/
│
├── Superstore_Analysis_Individual_Cells.ipynb
├── superstore_raw.csv
├── README.md
└── requirements.txt
```

## Analysis Performed

The notebook performs the following analysis:

1. Loads the Superstore CSV dataset.
2. Displays the first rows of the dataset.
3. Calculates total sales for each `Category`.
4. Visualizes total sales by category using a bar chart.
5. Visualizes profit distribution using a boxplot.
6. Creates a scatter plot of `Discount` vs `Profit`.
7. Calculates a correlation matrix for numerical columns.
8. Visualizes the correlation matrix using a heatmap.
9. Calculates total profit for each category.
10. Identifies the category with the highest total profit.
11. Identifies the category with the highest total sales.
12. Calculates the correlation between discount and profit.

## Key Results

Based on the supplied 100-row dataset and the notebook's existing analysis:

- The category label **`Furniture`** has the highest total sales among the exact category labels in the dataset, with approximately **5,487.73** in sales.
- The category label **`TECHNOLOGY`** has the highest total profit among the exact category labels, with approximately **432.63** in profit.
- The correlation between **Discount** and **Profit** is approximately **-0.28**.

> **Note:** The dataset contains category names with different capitalization, such as `Furniture`, `FURNITURE`, and `furniture`. The notebook groups the values exactly as they appear, so these capitalization variants are treated as separate categories.

## How to Run

### Option 1: Google Colab

1. Open `Superstore_Analysis_Individual_Cells.ipynb` in Google Colab.
2. Upload `superstore_raw.csv` when the notebook asks for the file.
3. Run the cells from top to bottom.

### Option 2: Jupyter Notebook

1. Install the required packages:

```bash
pip install -r requirements.txt
```

2. Open the notebook in Jupyter Notebook or JupyterLab.
3. Place `superstore_raw.csv` in the same working folder.
4. Run the notebook cells.

> The current notebook uses `google.colab.files.upload()` for file selection, so the file-upload cell is designed for Google Colab. For local Jupyter execution, the dataset-loading cell may need to be changed to read `superstore_raw.csv` directly.

## Author

**Dheen Seenivasan S**  
**III-BCA**  
**Roll No.: 15**
