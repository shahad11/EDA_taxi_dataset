# EDA_taxi_dataset
Exploratory data analysis (EDA) on a taxi dataset. It includes the following steps:

1) Load the dataset.
2) Inspect the data for any null values or outliers.
3) Calculate new features such as weekday, month, pickup hour, and trip duration.
4) Visualize the data using various plots, such as boxplots, bar charts, and histograms.
5) Identify patterns and trends in the data.

## Univariate Analysis
Univariate analysis examines individual variables or columns one at a time to understand their distributions and characteristics.

- The code uses df['rate_code'].value_counts() to count the occurrences of each rate code.
- It uses df['payment_type'].value_counts() to count the occurrences of each payment type.
- It identifies and prints the records with negative trip fare and near-zero trip distance.
- It calculates and prints the minimum non-zero trip fare in the dataset.
- The code converts the 'pickup_time' and 'dropoff_time' columns to datetime objects.
- It extracts additional time-related features, such as weekday, month, weekday number, and pickup hour.
- The code computes the trip duration by finding the difference between 'dropoff_time' and 'pickup_time' and assigns it to a new column 'trip_duration'.
- It calculates the average speed for each trip and adds an 'average_speed' column to the DataFrame.
- The code creates various visualizations to analyze the distributions and patterns of trip duration, trip distance, and speed. It identifies outliers and unusual patterns in the data.
## Bivariate Analysis
Bivariate analysis explores the relationships between pairs of variables.

- The code visualizes trip duration against various factors like the hour of the day, weekday, and month.
- It examines how trip distance varies with the hour of the day and the weekday.
- It investigates the relationship between trip fare and trip distance, weekday, pickup hour, and tip amount.


  
- Lastly, the code generates a correlation heatmap to show the relationships between numerical variables in the dataset, highlighting correlations between columns such as trip distance, average speed, trip fare, tip amount, and toll amount.

- The analysis provides insights into the dataset's distribution, patterns, and relationships, which can be valuable for making data-driven decisions or further data processing
