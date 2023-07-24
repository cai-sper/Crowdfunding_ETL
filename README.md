# Project 2: Crowdfunding ETL

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