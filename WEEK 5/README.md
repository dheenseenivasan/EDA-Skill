# Healthcare Data Analysis & EDA

## 📊 Project Overview

This project performs **Exploratory Data Analysis (EDA) on healthcare patient data** using Python. The analysis focuses on patient demographics, medical conditions, admission types, medical codes, billing amounts, admission and discharge dates, and hospital stay duration.

The project is implemented using **Pandas, Matplotlib, and Seaborn** in a Jupyter Notebook.

## 📁 Dataset

The dataset contains **500 records** with the following columns:

| Column | Description |
| ----------- | ------------------------ |
| `Patient_ID` | Unique patient identifier |
| `Gender` | Patient gender |
| `Age` | Patient age |
| `Medical_Condition` | Patient's medical condition |
| `Admission_Date` | Date of hospital admission |
| `Admission_Type` | Type of hospital admission |
| `Medical_Code` | Medical/diagnostic code associated with the patient |
| `Billing_Amount` | Healthcare billing amount |
| `Discharge_Date` | Date of hospital discharge |

## 🛠️ Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## 🔍 Analysis Performed

### 1. Data Exploration

- Loaded the healthcare dataset.
- Examined the dataset contents and column names.
- Checked the dataset shape.
- Inspected data types.
- Checked for missing values.
- Examined categorical values and basic statistics.

### 2. Missing Value Handling

The `Medical_Code` column contains **15 missing values**.

The missing medical codes are handled by replacing them with:

```python
df['Medical_Code'] = df['Medical_Code'].fillna('Unknown')
```

### 3. Date Data Cleaning

The `Admission_Date` and `Discharge_Date` columns are converted into datetime format for further analysis.

```python
df['Admission_Date'] = pd.to_datetime(df['Admission_Date'])
df['Discharge_Date'] = pd.to_datetime(df['Discharge_Date'])
```

### 4. Admission Type Cleaning

Admission types are cleaned by removing extra spaces and converting the values to lowercase.

```python
df["Admission_Type"] = (
    df["Admission_Type"]
    .str.strip()
    .str.lower()
)
```

The dataset contains three admission types:

- Routine
- Urgent
- Emergency

### 5. Hospital Stay Analysis

The project calculates the number of days each patient stayed in the hospital using the admission and discharge dates.

```python
df["Hos_Stay_Days"] = (
    df["Discharge_Date"] - df["Admission_Date"]
).dt.days
```

This helps analyze the distribution of hospital stay durations.

### 6. Billing Amount Analysis

Descriptive statistics are calculated for the `Billing_Amount` column to understand healthcare billing values.

The dataset has:

- **Minimum billing amount:** 2,300
- **Maximum billing amount:** 14,200
- **Average billing amount:** approximately 7,249

### 7. Medical Condition Analysis

The project examines the frequency of different medical conditions using value counts.

This helps understand the distribution of conditions represented in the dataset.

### 8. Admission Type vs. Medical Condition

A cross-tabulation is created between `Admission_Type` and `Medical_Condition` to examine how different medical conditions are distributed across admission types.

```python
pd.crosstab(
    df['Admission_Type'],
    df['Medical_Condition']
)
```

### 9. Age Analysis by Medical Condition

The average patient age is calculated for each medical condition.

```python
df.groupby('Medical_Condition')['Age'].mean()
```

This provides an overview of the average age associated with each condition in the dataset.

## 📈 Analysis Outputs

The notebook includes analysis for:

- Dataset structure and shape
- Data types
- Missing values
- Medical code completeness
- Admission type distribution
- Hospital stay duration
- Billing amount statistics
- Medical condition distribution
- Admission type vs. medical condition
- Average age by medical condition

## 📂 Project Structure

```text
Healthcare-EDA/
│
├── healthcare_raw.csv
├── Heathcare EDA.ipynb
└── README.md
```

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Install the required libraries

```bash
pip install pandas matplotlib seaborn jupyter
```

### 3. Open the notebook

```bash
jupyter notebook "Heathcare EDA.ipynb"
```

### 4. Run the cells

Make sure the `healthcare_raw.csv` dataset is available in the expected location before running the notebook.

## 🎯 Project Objective

The main objective of this project is to explore healthcare patient data and understand:

- Patient demographics
- Medical condition distribution
- Admission types
- Missing medical-code information
- Hospital stay duration
- Healthcare billing amounts
- Relationship between admission types and medical conditions
- Average patient age across medical conditions

## 👨‍💻 Author

**Dheen Seenivasan**

BCA Student
