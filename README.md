# NYC Airbnb Data Analysis

## 📌 Project Overview
This project analyzes and cleans New York City Airbnb listings data to explore pricing patterns, popular neighborhoods, and host activity.

## 📂 Dataset
- **Source:** [Inside Kraggle](https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata)
- Two versions included:
  - `Excel_Airbnb_Data.xlsx` (excel data)
  - `Cleaned_Airbnb_Data_wo_Index.csv` (cleaned data)
- The cleaned dataset removes duplicates, fixes inconsistent text formatting, and handles missing values.

## 🛠️ Data Cleaning Process

The dataset was cleaned in Python using Pandas. The following steps were performed:

1. **Deleting redundant columns**  
   - Removed columns that were not useful for analysis, such as ID fields or columns with constant values.

2. **Renaming columns for better readability**  
   - Converted column names to lowercase and replaced spaces with underscores for easier handling in code.

3. **Dropping duplicates**  
   - Identified and removed duplicate rows to ensure each listing is unique.

4. **Removing NaN values**  
   - Dropped rows with missing critical data (e.g., `price`, `room_type`).
   - Filled missing values for non-critical fields with appropriate defaults.

5. **Cleaning individual columns**  
   - Standardized text data (e.g., fixed inconsistent neighborhood spellings).
   - Converted date columns to datetime format.
   - Ensured numeric columns had correct data types.
