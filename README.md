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

# Step-by-Step: Appending Data from Multiple Sheets using Power Query

## 📌 Overview
This project demonstrates how to **append data from multiple sheets in Excel** using **Power Query**.  
The process ensures clean, consistent, and efficient data handling across multiple years or sources.

I learned and practiced this workflow under the guidance of **@Satish Dhawale**.

---

## ❖ Step-by-Step Process

### 1. Convert Each Sheet into a Table
- Go to each sheet in your workbook.
- Select the data and press **Ctrl + T** to convert it into a table.
- Ensure "My table has headers" is checked.

### 2. Rename Each Table
- Assign meaningful names:
  - `Table_2022`
  - `Table_2023`
  - `Table_2024`, etc.
- Use the **Table Design tab** to rename.

---

### 3. Open Power Query Editor
- Go to the **Data tab**.
- Click **Get Data → Launch Power Query Editor**.

### 4. Fetch All Tables in Workbook
- In the formula bar, enter:
=Excel.currentworlbook()
- This returns a list of all named tables in the workbook.

### 5. Select and Filter Required Tables
- Identify the tables you want to append.
- Filter by table name or remove unnecessary ones.

---

## 🔍 Viewing Table Data in Power Query

### 6. Do Not Click on the Table Name
- Avoid clicking directly on "Table" in the column.

### 7. Click on the Blank Space Beside Table Name
- Click the blank cell next to the word "Table".

### 8. View the Table Preview
- A preview of the table appears at the bottom of the Power Query window.

---

## 🔽 Expanding Table Data

### 9. Locate the Expand Icon
- Find the **Expand Button** next to columns containing records/tables.

### 10. Click the Expand Button
- A dialog box appears showing available fields.

### 11. Uncheck the Prefix Option
- Deselect **"Use original column name as prefix"**.

### 12. Click OK
- Expands fields with clean column names.

---

## ⚙️ Cleaning & Managing Steps

### 13. Reordering and Step Review
- Check the **Applied Steps pane** for unnecessary steps.
- Keep transformations clean.

### 14. Identifying Data Type Issues
- Symptoms:
- Dates not recognized (no calendar icon).
- Numbers not behaving as numeric.
- Columns appear as Text.

### 15. Fixing Data Types Efficiently
- Select all columns (**Ctrl + A**).
- Go to **Transform → Detect Data Type**.
- Power Query assigns correct types automatically.

### 16. Correcting Date Format
- Change **Date/Time → Date** if only date is needed.

### 17. Managing ‘Change Type’ Steps
- When re‑changing data types, choose **Replace current step** to avoid clutter.

---

## 📤 Loading Data into Excel

### 18. Load Final Data
- Click **Close & Load** to load into a new worksheet.

### 19. Load Data Using "Close & Load To"
- Choose **New Worksheet → Table option**.
- Click OK.

### 20. Understanding Table Name
- Output table is named after the query (e.g., Query1).
- Rename query to something meaningful like **All_Data**.

---

## ⚠️ Common Issues & Fixes

### Row Count Increasing After Refresh
- Cause: Output table included as source → duplication loop.
- Fix: In **Source step**, filter out the output table (e.g., All_Data).

---

## ➕ Adding New Tables in Future
- Add new worksheet (e.g., 2025).
- Convert to table (**Ctrl + T**).
- Refresh query → new table auto‑appended.

---

## 📝 Important Tips
1. Avoid blank rows/spaces.
2. Ensure new records are within the same table.
3. Add data directly to bottom of existing tables.
4. Never include output table as input again.

---

## 🚀 Impact
- Efficiently combines multiple sheets into one dataset.
- Ensures clean column names and correct data types.
- Prevents duplication issues during refresh.
- Scales easily when adding new tables.

---

## 📂 Files
- `Raw_MultiSheet_Data.xlsx` → Original workbook with multiple sheets.
- `Appended_Data.xlsx` → Final combined dataset.

---

## 🙏 Credits
This project was inspired and guided by **@Satish Dhawale**  
📧 info@satishdhawale.com  
🌐 [SkillCourse Data Analytics](https://skillcourse.in/data-analytics)
