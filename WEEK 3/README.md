# Shopify Stock Analysis

## Project Overview

This project performs exploratory data analysis (EDA) on Shopify stock market data using Python and Pandas. The analysis focuses on stock price movements, daily returns, trading volume, and identifying unusual/high-volume trading days.

The project is implemented in a Jupyter Notebook (`EDA-3.ipynb`) using the `shopify_stock.csv` dataset.

## Dataset

- **Dataset:** `shopify_stock.csv`
- **Records:** 2,469
- **Columns:** 7
- **Columns:** date, open, high, low, close, adj_close, volume

## Analysis Performed

The notebook includes the following analysis:

1. Loads the Shopify stock dataset.
2. Performs basic exploratory data analysis.
3. Converts the date column into a date format.
4. Checks for missing values and duplicate records.
5. Sorts the data by date.
6. Calculates **Daily Delta** to measure daily price change.
7. Calculates **Daily Return** as a percentage.
8. Analyzes trading-volume statistics.
9. Identifies anomalous/high-volume trading days.
10. Calculates the mean, variance, and standard deviation of daily returns.
11. Visualizes closing-price trends over time.
12. Visualizes trading-volume trends over time.
13. Displays the distribution of daily returns using a histogram.

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Structure

```text
Shopify-Stock-Analysis/
├── EDA-3.ipynb
├── shopify_stock.csv
├── README.md
└── requirements.txt
```

## How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd Shopify-Stock-Analysis
```

### 2. Install the required libraries

```bash
pip install -r requirements.txt
```

### 3. Open the notebook

```bash
jupyter notebook EDA-3.ipynb
```

Run the notebook cells from top to bottom.

## Project Objectives

The main objectives of this project are to:

- Understand the structure of Shopify stock data.
- Explore historical stock-price movements.
- Analyze daily price changes and returns.
- Examine trading-volume behavior.
- Identify unusual/high-volume trading days.
- Measure return variability using statistical measures.
- Visualize stock-price, volume, and return trends.

## Key Analysis Areas

### Stock Price Movement
The notebook examines closing-price trends across the available dates.

### Daily Returns
Daily returns are calculated to understand percentage-based changes in the stock price and their distribution.

### Trading Volume
Trading volume is analyzed using descriptive statistics and visualizations to understand periods of higher and lower market activity.

### Return Variability
Mean, variance, and standard deviation are calculated to describe the behavior and variability of daily returns.

### Visualizations
The project includes charts for:

- Closing price over time
- Trading volume over time
- Distribution of daily returns

## Author

**Dheen Seenivasan**  
BCA Student
