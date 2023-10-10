All the analysis and coding is in:
Project1-Group9\Uber-Weather-Project\project-1 - Q3.ipynb

All the images generated are stored at: 
Project1-Group9\Uber-Weather-Project\Images


# NYC Uber Pickup Patterns Analysis

This code performs an analysis of New York City (NYC) Uber pickup patterns during the first six months of 2015 throughout the day. It utilizes a dataset that includes various attributes related to pickups, such as date and time, borough, number of pickups, weather conditions (wind speed, visibility, temperature, dew point, sea level pressure, precipitation, snow depth), and a holiday indicator.

## Data Source

The analysis uses the following dataset:

- `clean.csv`: Contains NYC Uber pickup data, which has been cleaned and preprocessed for analysis.

## Analysis Overview

The code conducts the following analysis on NYC Uber pickup patterns:

### 1. Data Loading and Initial Examination

- Loads the cleaned dataset from the "clean.csv" file into a Pandas DataFrame.
- Provides information about the columns in the DataFrame.

### 2. Data Preparation

- Converts the "pickup_dt" column to the "datetime64" data type for time-based operations.
- Separates data into two categories: holidays and regular days.

### 3. Hourly Pickup Patterns Analysis (Holidays vs. Regular Days)

- Calculates the average number of pickups for each hour of the day, separately for holidays and regular days.
- Plots the average pickup patterns for each month separately for both holidays and regular days.

### 4. Hourly Pickup Patterns Analysis by Borough (Holidays vs. Regular Days)

- Calculates the average number of pickups for each hour of the day, separately for each borough and for holidays and regular days.
- Plots the average pickup patterns for each borough separately for both holidays and regular days.

### 5. Monthly Pickup Patterns Analysis by Borough (Holidays vs. Regular Days)

- Calculates the average number of pickups for each month, separately for each borough and for holidays and regular days.
- Plots the average pickup patterns for each borough separately for both holidays and regular days.

### 6. Hourly Analysis of Weather Variables (First 6 Months)

- Groups the data by month and hour of the day and calculates the average values of various weather-related variables (e.g., wind speed, temperature).
- Plots the average values of these variables by hour of the day for the first 6 months.

## Instructions

To use this script:

1. Ensure you have the following CSV file in the `Resources` directory:
   - `clean.csv` (containing the cleaned NYC Uber pickup data).

2. Run the script using Python.

3. The script will perform the analysis and generate various plots to visualize pickup patterns and weather-related trends.

4. The generated plots will be saved as image files in the `Images` directory.

Please make sure to have the necessary Python libraries installed, such as Pandas and Matplotlib, to execute this script successfully.
