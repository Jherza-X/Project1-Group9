# Project1-Group9
Group 9 - Mahsa, Emily, Jesus

# NYC Uber Pickup Data Analysis

This project analyzes New York City (NYC) Uber pickup data during the first six months of 2015 to provide insights and perform data cleaning and preprocessing. The analysis includes examining the dataset, handling missing values, creating new features, and preparing the data for further analysis.

## Data Source

The analysis is based on the following dataset:

- `uber_nyc_enriched.csv`: Contains NYC Uber pickup data, including information such as date and time of pickup, borough, number of pickups, weather-related data (speed, visibility, temperature, dew point, sea level pressure, precipitation, snow depth), and a holiday indicator.

## Overview

The analysis script performs the following tasks:

### 1. Data Loading and Initial Examination

- The CSV file `uber_nyc_enriched.csv` is loaded into a Pandas DataFrame.
- The information about columns in the DataFrame is displayed.

### 2. Data Cleaning

- Rows with missing values in the "borough" column are dropped to ensure data quality.
- The data type of the "pickup_dt" column is converted from "object" to "datetime64" for time-based operations.

### 3. Pickup Patterns Analysis

- Hourly and daily pickup patterns are calculated and stored in separate DataFrames.

### 4. Handling Missing Values

- Missing values in the dataset are filled in for the date "2015-01-01 00:00:00" for each borough. Missing values are filled with the average data for that hour in month 1.

### 5. Holiday Data Handling

- The "hday" column, representing holidays, is updated to include weekends as holidays.
- Specified dates are marked as holidays in the dataset.

### 6. Temperature Conversion

- The temperature data is converted from Fahrenheit to Celsius.

### 7. Data Export

- The cleaned and processed data is saved to a new CSV file named `clean.csv` for future analysis.

## Instructions

To use this script:

1. Ensure you have the following CSV file in the `Resources` directory:
   - `uber_nyc_enriched.csv`

2. Run the script using Python.

3. The script will perform the data analysis tasks and save the cleaned data to `clean.csv` in the `Resources` directory for further analysis.

4. You can then use the cleaned data for various data analysis and visualization tasks.

Please make sure to have the necessary Python libraries installed, such as Pandas and Matplotlib, to execute this script successfully.
