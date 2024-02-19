Summary of Changes to Original File:

Data Aggregation:

Three CSV files (JC-202303-citibike-tripdata.csv, JC-202304-citibike-tripdata.csv, JC-202305-citibike-tripdata.csv) have been merged into one.
Dataframes from each CSV file have been concatenated into a single dataframe.
Data Transformation:

Added columns for start_month and end_month extracted from the started_at and ended_at columns respectively.
Converted started_at and ended_at columns to datetime data type.
Extracted start_time and end_time from started_at and ended_at respectively, formatted in hours and minutes.
Calculated the duration of each trip in hours and rounded to two decimal places.
Removed the end_month column.
Added a new column Period of the day based on the start_time column, categorizing trips into "early morning," "morning," "afternoon," or "night."
File Output:

The modified dataframe has been written to a new CSV file named merged_citibike_data.csv, without including the index column.
These changes enhance the original dataset by providing additional insights such as trip duration, month-wise analysis, and categorization of trips based on the time of the day.