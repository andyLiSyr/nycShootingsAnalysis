# SQL Analysis on NYC Shootings Dataset

Shootings have become a growing problem in the United States. As a NYC resident, I wanted to know what the shootings situation was like in my city. I found a dataset on NYC Open Data that has all the past reported shootings from 2005-2022, this was perfect for my goal.

Link to Dataset: Click Here

## Questions to Answer

1. How many total reported shootings in NYC from 2017-2022?
  - 1.1 How many total shootings in each borough?
2. How many total shootings each year from 2017-2022?
  - 2.1 How many in each borough each year from 2017-2022?
3. Is there a monthly pattern in shootings?
4. What is the deadliest shooting incident from 2017-2022?
5. What is the distribution of shootings by each hour in 2022?
6. What is the distribution of shootings by victim and perpetrator demographics in 2022?
7. What are the top 5 precincts with the most shootings in 2022?

## Approach

#### Data Cleaning/Transformation

- Loaded the dataset into a Pandas dataframe in a Jupyter Notebook for data cleaning
- Checked for outlier values and nulls in each column, all outlier values were fixed and null values were filled in
- Removed unnecessary columns and filtered out rows of data that were not needed for my analyis
- Changed the structure of the original dataset by splitting it into two seperate CSV files that can be joined together
- Transformed the data by storing the CSV files in tables in a SQlite3 database

#### Data Analysis

- Performed analysis using combination of SQL queries and Pandas dataframes
- Visualized queries using libraries like Matplotlib and Seaborn
