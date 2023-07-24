# Project 2: Crowdfunding ETL
Team members: Cailin, Ellis, Kalyn, Kevin

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

=======

# Create the Crowdfunding Database

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