# Customer-Personality-Analysis-Data-Cleaning-Preprocessing
This project focuses on cleaning and preprocessing the Customer Personality Analysis dataset using Python (Pandas). The raw dataset contained missing values, duplicate records, inconsistent data formats, and other quality issues that were identified and resolved to prepare the data for further analysis

---

## 🎯 Objective

The objective of this project is to transform raw customer data into a clean, consistent, and analysis-ready dataset by applying standard data preprocessing techniques.

---

## 📂 Dataset

**Dataset Name:** Customer Personality Analysis

**Source:** Kaggle

The dataset contains customer demographic details, purchasing behavior, campaign responses, and spending across various product categories.

---

## 🛠️ Technologies Used

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Missingno
- Jupyter Notebook
- VS Code

---

## 📦 Libraries Installed

```bash
pip install pandas numpy matplotlib seaborn missingno scikit-learn openpyxl jupyter

---

# 📋 Data Cleaning Workflow

## 1. Dataset Import

- Loaded the CSV dataset using Pandas.
- Verified successful import.

```python
pd.read_csv()
```

---

## 2. Initial Data Exploration

Performed an initial assessment to understand the dataset.

Checked:

- Number of rows and columns
- Data types
- Missing values
- Duplicate records
- Statistical summary

Functions used:

- head()
- tail()
- info()
- describe()
- shape

---

## 3. Missing Value Analysis

Identified missing values using:

```python
df.isnull().sum()
```

Also visualized missing values using the **Missingno** library.

### Missing values were handled by:

- Median imputation for numerical columns
- Mode imputation for categorical columns

---

## 4. Duplicate Record Removal

Checked duplicate rows using

```python
df.duplicated().sum()
```

Removed duplicates using

```python
drop_duplicates()
```

---

## 5. Column Name Standardization

Renamed columns to improve consistency.

Changes made:

- Converted to lowercase
- Removed spaces
- Replaced spaces with underscores
- Removed unnecessary special characters

Example

Before

```
Year Birth
```

After

```
year_birth
```

---

## 6. Data Type Correction

Verified and corrected incorrect data types.

Examples

- Date columns converted to datetime
- Numeric columns converted to integer or float
- Object columns standardized

---

## 7. Text Standardization

Cleaned categorical text values by

- Removing leading spaces
- Removing trailing spaces
- Standardizing capitalization
- Fixing inconsistent text formatting

Example

Before

```
 married
MARRIED
Married
```

After

```
Married
```

---

## 8. Outlier Detection & Removal
- Detected outliers in the *income* column using the Interquartile Range (IQR) method.
- Removed records with extreme values outside the acceptable range.

---

## 9. Final Data Validation

Performed final quality checks.

Verified

- No duplicate rows
- Correct data types
- Consistent formatting
- Missing values handled
- Dataset ready for analysis

---

## 10. Export Clean Dataset

Saved cleaned dataset as

```
customer_personality_cleaned.csv
```

---

# 📊 Data Quality Report

The following preprocessing steps were completed:

✔ Missing values identified and treated

✔ Duplicate records removed

✔ Column names standardized

✔ Data types corrected

✔ Date columns formatted

✔ Text values standardized

✔ Outliers detected and treated

✔ New features created

✔ Clean dataset exported

---

# 📈 Skills Demonstrated

- Data Cleaning
- Data Preprocessing
- Exploratory Data Analysis
- Missing Value Treatment
- Duplicate Handling
- Feature Engineering
- Data Validation
- Data Quality Assessment
- Python Programming
- Pandas
- NumPy
- Data Visualization

---

# 📚 Key Python Functions Used

```
read_csv()

head()

tail()

info()

describe()

shape

isnull()

fillna()

drop_duplicates()

astype()

to_datetime()

rename()

str.lower()

str.replace()

get_dummies()

to_csv()
```
---

# 👩‍💻 Author

**Deepashree M**

Aspiring Data Analyst | Python | SQL | Power BI | Excel | Data Visualization
