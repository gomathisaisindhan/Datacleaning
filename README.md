# Datacleaning
Cleaned and preprocessed a raw sales dataset using Excel. Removed duplicates, handled missing values, standardized text and date formats, and ensured data consistency for accurate analysis and dashboard creation.
# 🧹 Task 1: Data Cleaning & Preprocessing — Sales Data

## 🎯 Objective
To clean and prepare a raw sales dataset by removing errors, fixing missing values, and ensuring data consistency for further analysis and visualization.

## 🛠 Tools Used
- Microsoft Excel (for data cleaning and formatting)

## 📋 Steps Performed
### 1️⃣ Removed Duplicates
- Used Data → Remove Duplicates.
- ✅ No duplicate rows were found in the dataset.

### 2️⃣ Handled Missing Values
| Column | Action Taken |
|:--|:--|
| phone | Filled 1 blank with “Unknown”. |
| state | Filled 1,486 blanks using nearby city or country values. |
| postalcode | Inferred from city or filled as “N/A” if not available. |
| territory | Filled 1,074 blanks with “Unassigned”. |

### 3️⃣ Standardized Text Values
- Ensured consistent casing (e.g., Tamil Nadu, not tamil nadu).
- Trimmed extra spaces using Excel’s TRIM() function.

### 4️⃣ Date Format Standardization
- Converted all orderdate values to dd-mm-yyyy format.

### 5️⃣ Data Type Check
| Column Type | Columns |
|:--|:--|
| Numeric | sales, quantityordered, priceeach, etc. |
| Text | state, city, country, territory, etc. |
| Date | orderdate |

All columns have correct and consistent data types ✅.

### 6️⃣ Outlier Check
- Verified numeric columns (sales, priceeach, etc.) for abnormal or negative values — none found.

## 📊 Final Dataset Overview
| Metric | Count |
|:--|--:|
| Rows | 2,823 |
| Columns | 24 |
| Missing Values | 0 |
| Duplicates | 0 |
| Format | .xlsx (Excel Cleaned Data) |

## 🧾 Output Files
- cleaned_data.xlsx → Initial cleaned version
- sales_data_cleaned_final.xlsx → Final verified version

## 💡 Key Learning Outcomes
- Handling missing values using logical imputation in Excel
- Identifying and removing duplicates
- Standardizing inconsistent text and date formats
- Ensuring clean, ready-to-analyze dataset for dashboards
