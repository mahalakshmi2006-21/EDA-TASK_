EDA-TASK_6
Exploratory Data Analysis (EDA) – Healthcare Dataset
1. Project Overview
This project performs Exploratory Data Analysis (EDA) on a healthcare dataset using Python. It explores patient demographics, medical conditions, admission types, admission and discharge dates, length of stay, and billing amounts. The project includes data inspection, data cleaning, summary statistics, grouped analysis, and visualizations.
2. Objectives
- Understand the dataset structure, columns, data types, and size.
- Identify and handle missing values.
- Standardize admission-type labels.
- Convert admission and discharge dates to datetime format.
- Calculate patient length of stay.
- Analyze billing amounts and average age by medical condition.
- Compare medical conditions by gender and admission type.
- Visualize admission counts, billing distributions, monthly admissions, and correlations.
3. Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab
4. Dataset
The project uses healthcare_data_for_task.csv.
- Rows: 1,000
- Original columns: 10
- Columns after feature engineering: 11
Dataset Columns
Column	Description
Patient_ID	Unique patient identifier
Age	Patient age
Gender	Patient gender
Blood_Type	Patient blood type
Medical_Condition	Recorded medical condition
Medical_Code	Code associated with the medical condition
Date_of_Admission	Date the patient was admitted
Discharge_Date	Date the patient was discharged
Admission_Type	Emergency, Elective, or Urgent
Billing_Amount	Patient billing amount
Stay_Date	Calculated length of stay in days


Before running: Place healthcare_data_for_task.csv in the notebook's working directory, or update the file path in the data-loading cell. The original notebook uses a Google Colab path: /content/healthcare_data_for_task.csv.
5. Analysis Workflow
1. Import the required Python libraries and load the CSV file.
2. Preview the data and inspect its shape, columns, and data types.
3. Check for missing values and replace missing Medical_Code values with Unknown.
4. Standardize Admission_Type values by trimming spaces and applying title case.
5. Convert admission and discharge dates to datetime format.
6. Create Stay_Date by subtracting the admission date from the discharge date.
7. Calculate billing summary statistics.
8. Analyze average age by medical condition and gender counts by condition.
9. Create visualizations to explore admission types, billing amounts, monthly admissions, and correlations.
6. Key Results
- The dataset contains 1,000 rows and 10 original columns.
- There are 30 missing values in Medical_Code; these are filled with Unknown.
- Admission-type counts:
  - Emergency: 381
  - Elective: 368
  - Urgent: 251
- Billing amount statistics:
  - Mean: 77,117.52
  - Median: 77,293.90
  - Minimum: 5,568.16
  - Maximum: 149,921.80
- Average age by medical condition:
  - Arthritis: 52.67
  - Asthma: 49.92
  - Diabetes: 53.13
  - Heart Disease: 52.18
  - Hypertension: 51.40
Note: Billing values are reported in the dataset's original units.
7. Visualizations
The notebook includes the following charts:
1. Admission Type Counts – compares Emergency, Elective, and Urgent admissions.
2. Total Billing by Medical Condition and Admission Type – stacked bar chart of total billing amounts.
3. Billing Distribution by Medical Condition – violin plot comparing billing distributions.
4. Monthly Patient Admissions – line chart showing admission counts by month.
5. Correlation Heatmap – shows correlations between age, length of stay, and billing amount.
8. Conclusion
This project summarizes healthcare records and explores admission patterns, billing variation, and age differences across medical conditions. It also performs basic data preparation by handling missing medical codes, standardizing admission labels, converting date columns, and calculating length of stay. Further work could examine outliers, validate date consistency, and investigate factors associated with higher billing amounts.
9. How to Run
1. Download or place healthcare_data_for_task.csv in the working directory.
2. Open the notebook in Jupyter Notebook or Google Colab.
3. Update the CSV path if required.
4. Run all cells from top to bottom.
5. Add the README and notebook to your project repository. Include the dataset only if you are permitted to share it.
Note: The results reflect the outputs saved in the supplied notebook. If the dataset or code changes, rerun the notebook and update the results accordingly.
