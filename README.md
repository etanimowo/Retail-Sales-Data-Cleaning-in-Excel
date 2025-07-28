## Retail Sales Data Cleaning in Excel

## Table of Content
- [Project Overview](#project-overview)
- [Objective](#objective)
- [Data Source](#data-source)
- [Tools Used](#tools-used)
- [Initial Assessment](#initial-assessment)
- [Handling Missing Values](#handling-missing-values)
- [Standardizing Formats](#standardizing-formats)
- [Fixing Dates](#fixing-dates)
- [Removing Duplicates](#removing-duplicates)
- [Data Type Corrections](#data-type-corrections)
- [Final Review](#final-review)
- [Conclusion](#conclusion)

  
### Project Overview
This project focused on cleaning a retail sales dataset with over 5,000 records using Microsoft Excel. The data contained common issues such as missing values, inconsistent formatting, duplicates, and invalid entries.

---
### Objective
The goal of this project is to clean and prepare a messy dataset of retail transactions containing over 5,000 rows. The retail dataset had issues such as missing values, inconsistent formats, duplicated entries, and incorrect data types. I used Microsoft Excel to clean and standardize the data to make it ready for analysis.

---
### Data Source
The dataset used for this project was gotten from a retail shop – (dirty_retail_dataset.xlsx). It consisted of over 5,000 rows representing customer name, email, purchase date, product, quantity, price, and city.

### Tools Used
- Microsoft Excel
- Excel functions: PROPER(), DATEVALUE()
- Data Validation, Filters, Remove Duplicates, and Conditional Formatting

---
### Initial Assessment
The first step in any data cleaning project is to have a proper understand of the dataset being worked upon.  Therefore, I began the data cleaning by opening the retail dataset and scanning through the columns: Customer Name, Email, Purchase Date, Product, Quantity, Price, and City to gain clarity and after careful observation. I observed several issues like:
- Missing values in Email, Quantity, and Price columns.
- Inconsistent date formats and invalid placeholders like “N/A”.
- Product names with inconsistent capitalization and spelling variations.
- Duplicate records.
- City names with inconsistent capitalization (e.g., "philadelphia" vs. "Philadelphia").

<img width="622" height="332" alt="clean1" src="https://github.com/user-attachments/assets/0ec77ee7-0a3b-4ddf-89f2-60b203ef353e" />

---
### Handling Missing Values
Next for me is to handle the missing values.  I used Excel’s filters and conditional formatting to identify and highlight blank or “N/A” entries like:
- Missing Email, I marked them as “Unknown” to preserve the row.
- Blank Quantity values were replaced with 1 as a default assumption.
- For Price, rows with “N/A” or blank prices were flagged for potential removal or correction depending on other information available.

---
### Standardizing Formats
There is need for me to standardize Product and City names:
- I used the LOWER and PROPER functions in Excel to fix inconsistent capitalization in Product and City columns.
- I created a new column called “Clean Product” to correct variants (e.g., “laptop” and “LAPTOP” were all changed to “Laptop”).

---
### Fixing Dates
Also, there is need to format the Purchase Date column.  I used Excel’s DATEVALUE function to convert text-based dates into proper date formats. Invalid entries like “N/A” were filtered and replaced with blanks.

---
### Removing Duplicates
Using the “Remove Duplicates” feature in Excel (under Data > Data Tools), I selected all columns to remove exact duplicate rows. This helped reduce redundant data and potential skew in analysis.

<img width="488" height="286" alt="clean5" src="https://github.com/user-attachments/assets/efebb766-ae44-4a62-aeba-49d7638756fe" />

---
### Data Type Corrections
I ensured the following:
- Quantity and Price columns were formatted as Number (with appropriate decimal places).
- Purchase Date was set to Date format (e.g., mm/dd/yyyy).

---
### Final Review
After applying the above transformations, and getting all the missing price values replaced. I reviewed the cleaned data:
- No missing or invalid critical fields
- Consistent product and city names
- Uniform date formatting
- Clean numeric columns
- Duplicates removed
Finally, the cleaned retail dataset is then saved as cleaned_retail_data.xlsx.

<img width="596" height="256" alt="dirty   cleaned dataset" src="https://github.com/user-attachments/assets/0ccbdd25-11b0-4d03-8cd7-b35b9836b19e" />

- [⬇️ Download dirty_retail_dataset.xlsx](./dirty_retail_dataset.xlsx)  
  Raw, unprocessed dataset containing missing values, inconsistent formats, and duplicates.

- [✅ Download cleaned_retail_dataset.xlsx](./cleaned_retail_dataset.xlsx)  
  Cleaned and standardized version of the dataset, ready for analysis.

---
### Conclusion:
In conclusion, data cleaning is essential part of data analysis project. This retail sales project demonstrated my ability to identify and correct a wide range of data quality issues using Microsoft Excel. It helped to ensuring that the retail dataset is reliable and analysis-ready, showcasing strong attention to detail and data cleaning skills using different Excel functions.

---


