# Shopify Stock Data Analysis & Visualization

## 📊 Project Overview

This project analyzes and visualizes historical **Shopify stock market data** using Python. The analysis focuses on stock price movements, trading volume, moving averages, daily returns, and volatility.

The project is implemented using **Pandas, NumPy, Matplotlib, and Seaborn** in a Jupyter Notebook.

## 📁 Dataset

The dataset contains **2,469 records** with the following columns:

| Column      | Description              |
| ----------- | ------------------------ |
| `date`      | Trading date             |
| `open`      | Opening stock price      |
| `high`      | Highest price of the day |
| `low`       | Lowest price of the day  |
| `close`     | Closing stock price      |
| `adj_close` | Adjusted closing price   |
| `volume`    | Number of shares traded  |

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## 🔍 Analysis Performed

### 1. Data Exploration

* Loaded the Shopify stock dataset.
* Examined the first few records.
* Checked dataset information and statistics.
* Checked the dataset shape.
* Converted the `date` column into a datetime format.
* Sorted the data chronologically.

### 2. Stock Price Visualization

Visualized the following prices over time:

* Open
* High
* Low
* Close

This helps understand Shopify's historical stock-price movement.

### 3. Trading Volume Analysis

The project visualizes **trading volume over time** to observe changes in the number of shares traded.

### 4. Moving Averages

Two moving averages are calculated:

* **20-day Moving Average (MA20)**
* **50-day Moving Average (MA50)**

These are compared with the closing price to visualize price trends.

### 5. Daily Returns

Daily stock returns are calculated using:

```python
df["Daily_Return"] = df["close"].pct_change()
```

A histogram with KDE is used to visualize the distribution of daily returns.

### 6. Volatility Analysis

The project calculates volatility using the standard deviation of daily returns.

It also calculates:

* **20-day rolling volatility**
* **100-day rolling volatility**

These are plotted over time to visualize changes in Shopify's stock-price volatility.

## 📈 Visualizations

The notebook produces visualizations for:

* Shopify Open, High, Low & Close Prices
* Trading Volume
* 20-Day Moving Average
* 50-Day Moving Average
* Moving Averages vs. Closing Price
* Daily Return Distribution
* Rolling Volatility
* 20-Day Rolling Volatility
* 100-Day Rolling Volatility

## 📂 Project Structure

```text
Shopify-Stock-Analysis/
│
├── shopify_stock.csv
├── Shopify_Visulaization.ipynb
└── README.md
```

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Install the required libraries

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

### 3. Open the notebook

```bash
jupyter notebook Shopify_Visulaization.ipynb
```

### 4. Run the cells

Make sure the CSV dataset is available in the expected location before running the notebook.

## 🎯 Project Objective

The main objective of this project is to explore historical Shopify stock data and understand:

* Stock price trends
* Trading activity
* Moving averages
* Daily price returns
* Market volatility

## 👨‍💻 Author

**Dheen Seenivasan**

BCA Student
