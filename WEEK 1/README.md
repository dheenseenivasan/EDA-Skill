Ecommerce Order Data Analysis

Project Overview

This project performs basic data inspection and preprocessing on an Ecommerce Order dataset using Python and Pandas.

The project is implemented in a Jupyter Notebook and focuses on understanding the structure and quality of the dataset through data preview, information, descriptive statistics, missing-value checks, duplicate checks, data-type inspection, and a simple gender-value standardization step.

Dataset

Dataset file: Ecommerce_Order_Test_Dataset(1).csv

The dataset contains 101 records and 13 columns.

Columns

Column

Description

Order_ID

Unique order identifier

Order_Date

Date on which the order was placed

Delivery_Date

Date on which the order was delivered

Customer_Name

Customer identifier/name

Gender

Customer gender

City

Customer city

Category

Product category

Product

Product purchased

Payment_Mode

Payment method used

Quantity

Quantity ordered

Unit_Price

Price per unit

Discount

Discount applied to the order

Rating

Customer rating

Technologies Used

Python

Pandas

Jupyter Notebook

Analysis Performed

The notebook includes the following steps:

Import the Pandas library.

Load the ecommerce order CSV dataset.

Display the first few records using head().

Inspect the dataset structure using info().

Generate descriptive statistics using describe().

Check for missing values using isnull().

Check for duplicate records using duplicated().

Inspect the data types of each column using dtypes.

Standardize the Gender column using capitalization with:

df['Gender'] = df['Gender'].str.capitalize()

Project Structure

Ecommerce-Order-Data-Analysis/
│
├── Super_store(1).ipynb
├── Ecommerce_Order_Test_Dataset(1).csv
├── README.md
└── requirements.txt

How to Run

1. Clone the repository

git clone <your-github-repository-url>

2. Install the required package

pip install -r requirements.txt

3. Open the notebook

jupyter notebook

Open:

Super_store(1).ipynb

4. Run the cells

Run the notebook cells from top to bottom to reproduce the data inspection and preprocessing steps.

Objective

The objective of this project is to practice basic ecommerce dataset handling using Pandas, including data loading, exploration, quality checks, and simple data preprocessing.

Author

Dheen Seenivasan

BCA Student
