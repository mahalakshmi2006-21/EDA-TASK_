# 🏥 EDA-TASK_6
# Exploratory Data Analysis (EDA) – Healthcare Dataset

## 1. Project Overview

This project performs Exploratory Data Analysis (EDA) on a healthcare dataset using Python. It explores patient demographics, medical conditions, admission types, hospital stay duration, and billing amounts. The project includes data cleaning, statistical analysis, and data visualization to identify useful patterns in healthcare records.

## 2. Objectives

- Inspect the dataset structure, columns, and data types.
- Identify and handle missing values.
- Clean and standardize admission-type labels.
- Convert date columns into datetime format.
- Calculate patient length of stay.
- Analyze billing amounts and average age by medical condition.
- Compare medical conditions by gender and admission type.
- Visualize admission trends, billing distributions, and correlations.

## 3. Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## 4. Dataset Information

**Dataset Name:** `healthcare_data_for_task.csv`

- Total Records: 1,000
- Original Columns: 10
- Columns After Feature Engineering: 11

### Dataset Columns

- `Patient_ID` – Unique patient identifier
- `Age` – Patient age
- `Gender` – Patient gender
- `Blood_Type` – Patient blood type
- `Medical_Condition` – Patient's medical condition
- `Medical_Code` – Medical condition code
- `Date_of_Admission` – Patient admission date
- `Discharge_Date` – Patient discharge date
- `Admission_Type` – Type of admission
- `Billing_Amount` – Patient billing amount
- `Stay_Date` – Length of hospital stay in days

## 5. Data Cleaning and Analysis

1. Imported the required Python libraries.
2. Loaded the healthcare dataset using Pandas.
3. Inspected the dataset using `head()`, `shape`, `columns`, and `info()`.
4. Checked missing values using `isnull().sum()`.
5. Replaced missing medical codes with `Unknown`.
6. Standardized admission-type labels.
7. Converted admission and discharge dates into datetime format.
8. Calculated hospital stay duration.
9. Analyzed billing statistics and average age by medical condition.
10. Created visualizations to understand healthcare trends.

## 6. Key Results

### Admission Type Counts

| Admission Type | Number of Patients |
|---|---:|
| Emergency | 381 |
| Elective | 368 |
| Urgent | 251 |
| **Total** | **1,000** |

### Billing Amount Statistics

| Statistic | Value |
|---|---:|
| Mean | 77,117.52 |
| Median | 77,293.90 |
| Minimum | 5,568.16 |
| Maximum | 149,921.80 |

### Average Age by Medical Condition

| Medical Condition | Average Age |
|---|---:|
| Arthritis | 52.67 |
| Asthma | 49.92 |
| Diabetes | 53.13 |
| Heart Disease | 52.18 |
| Hypertension | 51.40 |

## 7. Visualizations

The project includes the following visualizations:

- **Admission Type Counts:** Compares different admission types.
- **Billing by Medical Condition:** Displays total billing amounts by condition and admission type.
- **Billing Distribution:** Uses a violin plot to compare billing distributions.
- **Monthly Patient Admissions:** Shows admission trends over time.
- **Correlation Heatmap:** Displays correlations between age, hospital stay duration, and billing amount.

## 8. Conclusion

This project provides insights into healthcare records by analyzing patient demographics, medical conditions, admission patterns, and billing amounts. Data cleaning and feature engineering help prepare the dataset for further analysis. The visualizations make it easier to understand patterns and relationships within the data.

## 9. How to Run

1. Download the healthcare dataset.
2. Open the notebook in Jupyter Notebook or Google Colab.
3. Upload `healthcare_data_for_task.csv`.
4. Update the dataset file path if required.
5. Run all cells in sequence to reproduce the analysis and visualizations.

---

**Project:** Healthcare Dataset – Exploratory Data Analysis  
**Programming Language:** Python
