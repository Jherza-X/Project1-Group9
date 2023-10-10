Q4. How would you estimate the impact the weather has on Uber pickups?    
### a.Do certain weather conditions lead to an increase or decrease in pickups? 
### b.Are there any correlations between weather variables and pickups?

All the analysis and coding is in:
Project1-Group9\Uber-Weather-Project\project-1 - Q4 NCY.ipynb
Project1-Group9\Uber-Weather-Project\project-1 - Q4 Manhattan.ipynb

All the images generated are stored at: 
Project1-Group9\Uber-Weather-Project\Images

### Analysis and Conclusion for Q4

We created a correlation matrix for all the data, focusing on Manhattan. 
The heatmap indicates a mild correlation between pickups and weather conditions. When 
examining monthly patterns, we discovered a strong positive correlation between pickups 
and warmer weather. In simple terms, as the temperature rises, pickup numbers increase. 
Notably, February, the coldest month, exhibits an inverse correlation with snow depth, 
meaning deeper snow leads to more pickups. In conclusion, some weather conditions may
 lead to an increase or decrease in pickups, however, further analysis is needed with 
 a bigger set of data.


## Data Preparation

The analysis begins with loading the cleaned Uber pickup dataset from the CSV file named `clean.csv`. To focus on Manhattan, the data is filtered accordingly.

## Correlation Analysis

The exploration comprises several facets:

### 1. Correlation Analysis

The relationship between weather conditions and Uber pickups is assessed using Pearson correlation coefficients (r-values). These coefficients measure the strength and direction of the linear relationship between two variables. Correlations are calculated between individual weather variables (e.g., temperature, precipitation, snow depth) and the number of Uber pickups.

Additionally, linear regression analyses for each weather variable are conducted. This allows visualization of the relationships more intuitively. For both regular and holiday days, regression lines are plotted to illustrate how changes in weather variables affect the number of pickups.

### 2. Monthly Analysis

Recognizing that weather patterns can vary significantly throughout the year, a monthly analysis is conducted. This involves calculating the average number of Uber pickups and the average values of weather variables for each month. These averages help identify monthly trends and their potential correlation with weather conditions.

Bar charts are created to graphically represent how both average pickups and weather variables fluctuate over the months. This provides a clear picture of any seasonality or patterns that may exist.

### 3. Correlation Heatmaps

To gain a holistic view of the correlations between weather variables and Uber pickups, correlation heatmaps are generated. These visualizations offer a color-coded representation of correlation strength. They allow identification of which weather variables exhibit strong or weak correlations with pickups for each month.

## Instructions

To use this script:

1. Ensure you have the following CSV file in the `Resources` directory:
   - `clean.csv` (containing the cleaned NYC Uber pickup data).

2. Run the script using Python.

3. The script will perform the analysis and generate various plots to visualize 

4. The generated plots will be saved as image files in the `Images` directory.

Please make sure to have the necessary Python libraries installed, such as Pandas and Matplotlib, to execute this script successfully.





