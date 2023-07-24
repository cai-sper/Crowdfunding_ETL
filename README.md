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




# Campaign DataFrame



# Contacts DataFrame



# Crowdfunding Database
