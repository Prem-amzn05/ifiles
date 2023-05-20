# PandasAssignment

Q1. How do you load a CSV file into a Pandas DataFrame?
Ans:  To load a CSV file into a Pandas DataFrame, you can use the read_csv() function. Here's an example:
import pandas as pd

df = pd.read_csv('filename.csv')
In the above code, replace 'filename.csv' with the path and name of your CSV file. Pandas will read the CSV file and create a DataFrame object df containing the data.

Q2. How do you check the data type of a column in a Pandas DataFrame?

Ans: To check the data type of a column in a Pandas DataFrame, you can use the dtypes attribute or the dtype method. Here's an example:

# Using dtypes attribute
print(df.dtypes)

# Using dtype method for a specific column
print(df['column_name'].dtype)

The dtypes attribute will display the data types of all columns in the DataFrame. You can access the data type of a specific column by using the dtype method and passing the column name.

Q3. How do you select rows from a Pandas DataFrame based on a condition?
Ans: To select rows from a Pandas DataFrame based on a condition, you can use boolean indexing. Here's an example:
# Select rows where the 'column_name' is greater than a certain value
selected_rows = df[df['column_name'] > value]

# Select rows where a condition is satisfied for multiple columns
selected_rows = df[(df['column1'] > value1) & (df['column2'] == value2)]

In the above code, replace 'column_name' with the name of the column you want to use for the condition, value with the desired threshold, and column1, value1, column2, value2 with the respective column names and values for the multiple conditions.

Q4. How do you rename columns in a Pandas DataFrame?

Ans: To rename columns in a Pandas DataFrame, you can use the rename() method. Here's an example:
# Rename a single column
df = df.rename(columns={'old_name': 'new_name'})

# Rename multiple columns
df = df.rename(columns={'old_name1': 'new_name1', 'old_name2': 'new_name2'})

In the above code, replace 'old_name' with the current name of the column and 'new_name' with the desired new name. You can specify multiple column renames by adding more key-value pairs in the dictionary passed to the columns parameter.

Q5. How do you drop columns in a Pandas DataFrame?
Ans: To drop columns in a Pandas DataFrame, you can use the drop() method. Here's an example:

# Drop a single column
df = df.drop('column_name', axis=1)

# Drop multiple columns
df = df.drop(['column_name1', 'column_name2'], axis=1)
In the above code, replace 'column_name', 'column_name1', 'column_name2', etc. with the names of the columns you want to drop. The axis=1 parameter specifies that you want to drop columns (as opposed to rows).

Q6. How do you find the unique values in a column of a Pandas DataFrame?
Ans: To find the unique values in a column of a Pandas DataFrame, you can use the unique() method. Here's an example:

unique_values = df['column_name'].unique()
print(unique_values)
In the above code, replace 'column_name' with the name of the column for which you want to find the unique values. The unique() method will return an array containing all the unique values in that column.

Q7. How do you find the number of missing values in each column of a Pandas DataFrame?
Ans: To find the number of missing values in each column of a Pandas DataFrame, you can use the isnull() and sum() methods. Here's an example:

missing_values_count = df.isnull().sum()
print(missing_values_count)

The isnull() method checks each element in the DataFrame and returns a DataFrame of the same shape, where each element is True if it is missing (NaN) and False otherwise. The sum() method then sums up the number of True values for each column, giving you the count of missing values in each column.

Q8. How do you fill missing values in a Pandas DataFrame with a specific value?
Ans:  To fill missing values in a Pandas DataFrame with a specific value, you can use the fillna() method. Here's an example:

df = df.fillna(value)

Replace value with the specific value you want to use to fill the missing values. This method will replace all missing values (NaN) in the DataFrame with the specified value.


Q9. How do you concatenate two Pandas DataFrames?

Ans: To concatenate two Pandas DataFrames, you can use the concat() function. Here's an example:

concatenated_df = pd.concat([df1, df2])

In the above code, df1 and df2 are the DataFrames you want to concatenate. The concat() function will combine the rows of the two DataFrames, creating a new DataFrame concatenated_df with the concatenated result.

Q10. How do you merge two Pandas DataFrames on a specific column?
Ans: To merge two Pandas DataFrames on a specific column, you can use the merge() function. Here's an example:

merged_df = pd.merge(df1, df2, on='common_column')

In the above code, df1 and df2 are the DataFrames you want to merge, and 'common_column' is the name of the column on which you want to merge the DataFrames. The merge() function will combine the rows of the DataFrames based on matching values in the specified column, creating a new DataFrame merged_df with the merged result.

Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?
Ans: To group data in a Pandas DataFrame by a specific column and apply an aggregation function, you can use the groupby() method. Here's an example:

grouped_data = df.groupby('column_name').agg({'aggregated_column': 'aggregation_function'})

Replace 'column_name' with the name of the column you want to group by. 'aggregated_column' should be replaced with the column you want to perform the aggregation on. Finally, 'aggregation_function' should be replaced with the desired aggregation function, such as 'sum', 'mean', 'count', etc. The resulting grouped_data will be a new DataFrame with the grouped data and the applied aggregation function.

Q12. How do you pivot a Pandas DataFrame?
Ans:  To pivot a Pandas DataFrame, you can use the pivot() method. Here's an example:

pivoted_df = df.pivot(index='index_column', columns='column_to_pivot', values='values_column')

Replace 'index_column' with the column you want to set as the index of the pivoted DataFrame. 'column_to_pivot' is the column whose unique values will become the new columns of the pivoted DataFrame. Finally, 'values_column' is the column containing the values to populate the new columns. The resulting pivoted_df will be a new DataFrame with the pivoted structure.

Q13. How do you change the data type of a column in a Pandas DataFrame?
Ans:  To change the data type of a column in a Pandas DataFrame, you can use the astype() method. Here's an example:

df['column_name'] = df['column_name'].astype(new_data_type)

Replace 'column_name' with the name of the column you want to change the data type of. 'new_data_type' should be replaced with the desired data type, such as 'int', 'float', 'str', etc. The astype() method will convert the values in the specified column to the new data type.

Q14. How do you sort a Pandas DataFrame by a specific column?
Ans:  To sort a Pandas DataFrame by a specific column, you can use the sort_values() method. Here's an example:

sorted_df = df.sort_values('column_name', ascending=True)

Replace 'column_name' with the name of the column you want to sort by. By default, the DataFrame will be sorted in ascending order. If you want to sort in descending order, set ascending=False. The resulting sorted_df will be a new DataFrame with the rows sorted based on the specified column.

Q15. How do you create a copy of a Pandas DataFrame?
Ans: To create a copy of a Pandas DataFrame, you can use the copy() method. Here's an example:
df_copy = df.copy()
The copy() method creates a deep copy of the DataFrame, meaning that changes made to the copy will not affect the original DataFrame and vice versa. The df_copy will be an independent copy of the original DataFrame df.

Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?
Ans: To filter rows of a Pandas DataFrame by multiple conditions, you can use boolean indexing with logical operators (& for "and" and | for "or"). Here's an example:

filtered_df = df[(condition1) & (condition2)]

Replace condition1 and condition2 with the desired conditions for filtering the DataFrame. You can use comparison operators (>, <, ==, etc.) to create the conditions. The resulting filtered_df will be a new DataFrame containing only the rows that satisfy both conditions.

Q17. How do you calculate the mean of a column in a Pandas DataFrame?
Ans: To calculate the mean of a column in a Pandas DataFrame, you can use the mean() method. Here's an example:

column_mean = df['column_name'].mean()
print(column_mean)

Replace 'column_name' with the name of the column for which you want to calculate the mean. The mean() method will return the average value of the specified column.

Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?

Ans: To calculate the standard deviation of a column in a Pandas DataFrame, you can use the std() method. Here's an example:

column_std = df['column_name'].std()
print(column_std)

Replace 'column_name' with the name of the column for which you want to calculate the standard deviation. The std() method will return the standard deviation of the specified column.

Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?

Ans: To calculate the correlation between two columns in a Pandas DataFrame, you can use the corr() method. Here's an example:
correlation = df['column1'].corr(df['column2'])
print(correlation)
Replace 'column1' and 'column2' with the names of the two columns for which you want to calculate the correlation. The corr() method will return the correlation coefficient between the two specified columns.

Q20. How do you select specific columns in a DataFrame using their labels?

Ans:  To select specific columns in a DataFrame using their labels, you can directly access those columns using square brackets ([]). Here's an example:

selected_columns = df[['column1', 'column2', 'column3']]

Replace 'column1', 'column2', and 'column3' with the labels of the columns you want to select. The resulting selected_columns will be a new DataFrame containing only the specified columns. Note that the column labels should be provided as a list inside the square brackets.



Q21. How do you select specific rows in a DataFrame using their indexes?
Ans: To select specific rows in a DataFrame using their indexes, you can use the .loc indexer. Here's an example:

selected_rows = df.loc[[index1, index2, index3]]
Replace index1, index2, index3, etc. with the specific indexes of the rows you want to select. The resulting selected_rows will be a new DataFrame containing only the specified rows.

Q22. How do you sort a DataFrame by a specific column?
Ans: To sort a DataFrame by a specific column, you can use the sort_values() method. Here's an example:

sorted_df = df.sort_values('column_name', ascending=True)

Replace 'column_name' with the name of the column you want to sort by. By default, the DataFrame will be sorted in ascending order. If you want to sort in descending order, set ascending=False. The resulting sorted_df will be a new DataFrame with the rows sorted based on the specified column.



Q23. How do you create a new column in a DataFrame based on the values of another column?
Ans: To create a new column in a DataFrame based on the values of another column, you can assign values to the new column using square brackets ([]). Here's an example:

df['new_column'] = df['existing_column'] * 2
Replace 'new_column' with the name you want to give to the new column and 'existing_column' with the name of the column you want to use for calculation. In the example, the new column will be created by multiplying the values of the existing column by 2.


Q24. How do you remove duplicates from a DataFrame?
Ans: To remove duplicates from a DataFrame, you can use the drop_duplicates() method. Here's an example:
df_no_duplicates = df.drop_duplicates()
The drop_duplicates() method will return a new DataFrame, df_no_duplicates, with duplicate rows removed. By default, it keeps the first occurrence of each duplicated row and removes the subsequent duplicates.



Q25. What is the difference between .loc and .iloc in Pandas?
Ans:  The main difference between .loc and .iloc in Pandas is the way they handle indexing.

.loc is primarily label-based and is used to access rows and columns in a DataFrame using their labels. It accepts label-based indexing, slicing, or boolean indexing using labels.

.iloc is primarily integer-based and is used to access rows and columns in a DataFrame using their integer positions. It accepts integer-based indexing, slicing, or boolean indexing using integer positions.

Here's an example to illustrate the difference:
# Using .loc
df.loc[2:4, 'column_name']  # Access rows 2 to 4 in 'column_name' using labels

# Using .iloc
df.iloc[2:4, 3]  # Access rows 2 to 3 in the 4th column using integer positions

In the .loc example, the slicing range 2:4 refers to the labels of the rows, while in the .iloc example, the slicing range 2:4 refers to the integer positions of the rows. Similarly, the column selection 'column_name' in .loc refers to the label of the column, while the column selection 3 in .iloc refers to the integer position of the column.




