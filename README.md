# Project 2: ETL Mini Project
## By Kalyn Aguiar, Kevin Jeong, Cailin Sperling, Ellis Zimmer

# Category and Subcategory DataFrames

## Create a Category that has the following columns: 

A "category_id" column that has entries going sequentially from "cat1" to "catn", where n is the number of unique categories.

A "category" column that contains only the category titles.

Export the category DataFrame as category.csv and save it to your GitHub repository.

## Create a Subcategory DataFrame that has the following columns: 

A "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn", where n is the number of unique subcategories

A "subcategory" column that contains only the subcategory titles

Export the subcategory DataFrame as subcategory.csv and save it to your GitHub repository.

## Description

I started by splitting the 'category & sub-category' column into separate columns in the crowdfunding_info_df dataframe. This was done using the .str.split method to separate the strings and place them in corresponding columns in the dataframe. To ensure only unique values are represented a for loop was used to append values into category and subcategory lists. The next step was to get the number of distinct values in the categories and subcategories lists. The unique values in each list were given a number id using numpy arrays. List comprehension allowed us to create values going sequentially from 'cat1' to 'catn' by adding 'cat' and 'subcat' to each number id. Finally, each dataframe was created with the number ids and lists. Category and Subcategory dataframes were exported as CSV files with the code provided.

![Category](https://github.com/cai-sper/Crowdfunding_ETL/assets/131548874/0a1b62a7-6bc8-46aa-ba36-1dcf074624d4)

![Subcategory](https://github.com/cai-sper/Crowdfunding_ETL/assets/131548874/50a16154-f058-48e0-95a2-34671ffb8be7)

# Contacts DataFrame
 
## Create a Campaign DataFrame that has the following columns:

Extract four digit ID number.

Check data types.

Convert "contact_id" column to an int64.

Extract name of the contact and add it to a new column

Extract email from the contacts and add values to a new column

Create copy of the contact_info_df with the 'contact_id', 'name', 'email' columns

Create a "first"name" and "last_name" column with the first and last names from the "name" column

Drop contact_name column

Reorder columns

Check datatypes one last time, export as CSV file

# Crowdfunding Database

## Create the Crowdfunding Database

Inspect the four CSV files, and then sketch an ERD of the tables by using QuickDBDLinks to an external site..

Use the information from the ERD to create a table schema for each CSV file.

Note: Remember to specify the data types, primary keys, foreign keys, and other constraints.

Save the database schema as a Postgres file named crowdfunding_db_schema.sql, and save it to your GitHub repository.

Create a new Postgres database, named crowdfunding_db.

Using the database schema, create the tables in the correct order to handle the foreign keys.

Verify the table creation by running a SELECT statement for each table.

Import each CSV file into its corresponding SQL table.

Verify that each table has the correct data by running a SELECT statement for each.

## Description

We created a database schema in SQL for four tables: Category, Contacts, Subcategory, and Campaign. The four tables were created with four primary keys (category_id, contact_id, subcategory_id, cf_id) and three foreign keys connecting them together. We also created ERD to visualize the relationships between the tables.

# References

https://stackoverflow.com/questions/14745022/how-to-split-a-dataframe-string-column-into-two-columns

https://sparkbyexamples.com/pandas/pandas-convert-column-to-int/

https://stackoverflow.com/questions/43956335/convert-float64-column-to-int64-in-pandas

https://stackoverflow.com/questions/67394800/regex-to-extract-numbers-length-4-from-a-dataframe-column
