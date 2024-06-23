# Dataframe-Compare-Summary
Compare two dataframes and generated a mismatch report.


---
DataFrame Comparison and Summary Report
This script provides a comprehensive solution for comparing two dataframes using Dask and Pandas, and generating a detailed summary report of the differences. It includes the following features:
Data Generation: Creates sample dataframes with customizable columns and rows.
DataFrame Comparison: Compares two dataframes on specified join columns and identifies rows that are only in one dataframe or have mismatched values.
Report Generation: Produces a detailed report using PrettyTable, summarizing:
DataFrame information and summary
Columns present in one dataframe but not the other
Rows unique to each dataframe
Mismatched rows with specific column differences
Sample mismatched rows for quick review

Usage
1. Generate Sample Data: Modify the common_data and df2_additional dictionaries to customize the sample data.
2. Compare DataFrames: Use the compare_dataframes function to compare two dataframes.
3. Generate Report: Use the generate_report function to create a detailed comparison report.
Dependencies
dask
pandas
numpy
prettytable
datetime

# Example
- differences = compare_dataframes(ddf1, ddf2, join_column)
- report = generate_report(df1, df2, differences, join_column=join_column, sample_rows=sample_rows, mismatch_sample=mismatch_sample)
- print(report)
)
---
Feel free to customize further to better fit your project's specifics and goals.
