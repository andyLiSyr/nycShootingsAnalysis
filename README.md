# SQL Analysis on NYC Shootings Dataset

![NYC Logo](https://nycmbk.org/wp-content/uploads/2019/10/nyc-logo.png)

Shootings have become a growing problem in the United States. As a NYC resident, I wanted to know what the shootings situation was like in my city. I found a dataset on NYC Open Data that has all the past reported shootings from 2005-2022, this was perfect for my goal.

Link to Dataset: [Click Here](https://data.cityofnewyork.us/Public-Safety/NYPD-Shooting-Incident-Data-Historic-/833y-fsy8)

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
- Removed unnecessary columns and filtered out rows of data that were not needed for my analysis
- Changed the structure of the original dataset by splitting it into two seperate CSV files that can be joined together
- Transformed the data by storing the CSV files in tables in a SQLite3 database

#### Data Analysis

- Performed analysis using combination of SQL queries and Pandas dataframes
- Visualized queries using libraries like Matplotlib and Seaborn

## Files in this Repo

Data Folder
- NY_Shootings.csv: The original NYC shootings CSV dataset downloaded from NYC Open Data
- clean_nyc_shootings.ipynb: The data cleaning code for the original dataset
- clean_incidents.csv: One of the CSV files resulting from the data cleaning
- clean_shootings.csv: The other CSV file resulting from the data cleaning, clean_incidents.csv and clean_shootings.csv can be joined together
- nyc_shootings_db_setup.ipynb: The code for setting up the and storing the two csv files in two tables in a SQlite3 database

Analysis Folder
- nyc_shootings_analysis.ipynb: The analysis code on the two SQLite3 tables containing the NYC shootings data

Charts Folder: The folder contains all the visualizations created in the analysis code as image files
