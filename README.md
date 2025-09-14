# Data Wrangling: Cleaning and Merging HIV & HBV Datasets

## Overview
This project demonstrates **data wrangling and cleaning techniques** using two global health datasets:  
- **HBV (Hepatitis B Virus)** dataset  
- **HIV (Human Immunodeficiency Virus)** dataset  

The objective of this project is to **clean messy real-world data**, remove inconsistencies, and **merge multiple datasets** into a structured format suitable for further analysis.  

## Steps Performed:

# 1. Data Cleaning
For both HBV and HIV datasets:
- Read the raw datasets into Pandas DataFrames.  
- Reset and managed **indexing**.  
- Dropped unnecessary columns.  
- Renamed columns for clarity.  
- Rounded integer values where required.  
- Used **GroupBy** to aggregate annual deaths per **country and year** (solving the issue of duplicate entries).  

# 2. Data Export
- Saved the cleaned versions of both datasets into new CSV files.  

# 3. Data Merging & Wrangling
- Re-imported the cleaned datasets.  
- **Merged** the HIV and HBV datasets on the `Country/Region` and `Year` column.  
- Split data into columns:  
  - Annual deaths from HIV  
  - Annual deaths from HBV  
- Ensured the `Year` column was numeric to allow **sorting**.  
- Rearranged columns for readability.  
- Reset the index for consistency.  
- Filled missing values (`NaN`) with zeros.  

# 4. Final Output
- Produced a **clean, merged dataset** with:  
  - `Country/Region`  
  - `Year`  
  - `Annual Deaths (HIV)`  
  - `Annual Deaths (HBV)`  

This dataset can now be used for **analysis, visualization, and predictive modeling**.  

## Key Concepts Covered:
- Data Cleaning  
- Indexing and Column Management  
- GroupBy Aggregation  
- Handling Missing Values  
- Dataset Merging  
- Data Sorting and Rearrangement  

