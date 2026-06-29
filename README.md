Data Cleaning Summary
Dataset: Flipkart_sales.xlsx
Records: 50,000 rows × 8 columns

Cleaning Steps Performed
1.	Missing Value Treatment:
Identified blank cells across the dataset using  go to Special feature in Excel. Filled missing numeric values with the column median, and missing categorical values with the mode to maintain data distribution and integrity.

2.	Duplicate Removal:
 Used Excel's Remove Duplicates feature to identify and eliminate redundant rows based      on all columns. Removed 1,245 duplicate records, reducing dataset from 51,245 to 50,000 records while preserving data quality.

3.	Text Standardization:
Standardized inconsistent text entries across categorical columns (product category, ratings). Applied text-case functions to ensure uniformity in formatting, removing leading/trailing spaces and converting to consistent case formats.

4.	Date Format Conversion:
Converted all date columns to a standard format (YYYY-MM-DD). Resolved inconsistent date   representations and ensured all dates are recognized as datetime objects for proper chronological analysis.

5.	Data Type Validation:
Verified and corrected data types for all columns. Converted price columns to decimal, quantity to integer, ratings to float, and ensured date columns are datetime objects for proper calculations and filtering.

Tools & Techniques Used:

•	Go To Special (F5) and Find & Replace features to isolate and fill empty cells efficiently
•	Excel's Remove Duplicates function to identify redundant rows across all selected columns
•	Text functions (UPPER, LOWER, TRIM) for standardization and formatting consistency
•	Format Cells dialog to convert and validate data types across the dataset
•	Python Pandas functions (fillna, drop_duplicates, apply) for advanced cleaning operations
