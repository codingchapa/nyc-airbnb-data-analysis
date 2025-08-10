# NYC Airbnb Data Analysis

## 📌 Project Overview
This project analyzes and cleans New York City Airbnb listings data to explore pricing patterns, popular neighborhoods, and host activity.

## 📂 Dataset
- **Source:** [Inside Kraggle](https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata)

## 🛠️ Data Cleaning Process

The dataset was cleaned in Python using Pandas. The following steps were performed:

1. **Column Selection**  
   - Kept only the columns relevant for analysis:
     - `NAME`, `host id`, `host_identity_verified`, `host name`,
       `neighbourhood group`, `neighbourhood`, `lat`, `long`, `country`,
       `country code`, `instant_bookable`, `cancellation_policy`, `room type`,
       `Construction year`, `price`, `service fee`, `minimum nights`,
       `number of reviews`, `last review`
   - Dropped less relevant or redundant columns:
     - `reviews per month`, `review rate number`, `calculated host listings count`,
       `availability 365`, `house_rules`, `license`, `id`

2. **Renaming Columns for Readability**  
   - Converted column names to lowercase
   - Replaced spaces with underscores (`NAME` → `name`)

3. **Removing NaN Values**
   - Removed duplicates
   - Dropped rows with missing values in critical fields such as `price` and `room_type`.

5. **Cleaning Individual Columns**  
   - Standardized text values (e.g., neighborhood names)
   - Changed datatype from str to int for 'price'
   - Ensured numeric columns had the correct data types

6. **Additional Transformations**
   - Removed index column
   - Created a cleaned dataset saved as `Cleaned_Airbnb_Data_wo_Index.csv`
  
## Two versions included:
  - `Excel_Airbnb_Data.xlsx` (excel data)
  - `Cleaned_Airbnb_Data_wo_Index.csv` (cleaned data)
- The cleaned dataset removes duplicates, fixes inconsistent text formatting, and handles missing values.
