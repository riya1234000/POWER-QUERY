# Medical History Dataset Cleaning Project

## 📌 Overview
This project demonstrates **data cleaning techniques** applied to a raw medical dataset.  
The dataset contained patient demographics, lifestyle factors, and stroke risk indicators.  
The goal was to transform messy, inconsistent records into a clean dataset ready for analysis.

## 🛠️ Cleaning Steps
1. Removed null values from the `ID` column.
2. Converted `Data Collection Date` from `datetime` to `date` format.
3. Standardized gender values: replaced `F` → `Female`, `M` → `Male`.
4. Created a `Full Name` column by combining initials and last names.
5. Converted numeric marital status values:
   - `1` → `Happily Married`
   - `0` → `Single`

## 📊 Impact
- Improved **data integrity** by removing nulls.
- Enhanced **readability** with standardized formats.
- Enabled **better analysis** by converting categorical values into meaningful labels.

## 📂 Files
- `Medical History Raw Data.xlsx` → Original dataset
- `Medical History Cleaned Data.xlsx` → Cleaned dataset

## 🚀 How to Use
Clone the repository and explore the cleaned dataset for further analysis, visualization, or predictive modeling.

```bash
(https://github.com/riya1234000/POWER-QUERY/blob/main/1%20-%20Medical%20History%20Raw%20Data.xlsx)
