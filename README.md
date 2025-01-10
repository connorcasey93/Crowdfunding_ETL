# Crowdfunding_ETL
Project 2
Code found in Starter_File folder

The instructions for this mini project are divided into the following subsections:

Create the Category and Subcategory DataFrames
Create the Campaign DataFrame
Create the Contacts DataFrame
Create the Crowdfunding Database

Use code in ETL_Mini_Project_Ccasey.ipynb for the fist three subsections

Create the Category and Subcategory DataFrames 
 
  - Extract and transform the crowdfunding.xlsx
  - Create data frame that has columns with
        A "category_id" column that has entries going sequentially from "cat1" to "catn", where n is the number of unique categories
        A "category" column that contains only the category titles
- Export the category DataFrame as category.csv and save it to GitHub repository
- Extract and transform the crowdfunding.xlsx Excel data
- Create a subcategory DataFrame that has columns with
    A "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn", where n is the number of unique subcategories
    A "subcategory" column that contains only the subcategory titles
- Export the subcategory DataFrame as subcategory.csv and save it to GitHub repository

Create the Campaign DataFrame

- Extract and transform the crowdfunding.xlsx Excel data to create a campaign DataFrame has the following columns:
      The "cf_id" column
      The "contact_id" column
      The "company_name" column
      The "blurb" column, renamed to "description"
      The "goal" column, converted to the float data type
      The "pledged" column, converted to the float data type
      The "outcome" column
      The "backers_count" column
      The "country" column
      The "currency" column
      The "launched_at" column, renamed to "launch_date" and with the UTC times converted to the datetime format
      The "deadline" column, renamed to "end_date" and with the UTC times converted to the datetime format
      The "category_id" column, with unique identification numbers matching those in the "category_id" column of the category DataFrame
      The "subcategory_id" column, with the unique identification numbers matching those in the "subcategory_id" column of the subcategory DataFrame

 Create the Contacts DataFrame
 
 Extract and transform the data from the contacts.xlsx Excel data   
- Import the contacts.xlsx file into a DataFrame.
- Iterate through the DataFrame, converting each row to a dictionary.
- Iterate through each dictionary, doing the following:
- Extract the dictionary values from the keys by using a Python list comprehension.
- Add the values for each row to a new list.
- Create a new DataFrame that contains the extracted data.
- Split each "name" column value into a first and last name, and place each in a new column.
- Clean and export the DataFrame as contacts.csv and save it to your GitHub repository.

  Create the Crowdfunding Database
Create a new Postgres database, named crowdfunding_db.
Use code in crowdfunding_db_schema.sql for this subsection
- Using crowdfunding_db_schema.sql to create the tables in the correct order to handle the foreign keys.
- Verify the table creation by running each SELECT statement seperately in from project2_campaignquery.sql
- Import each CSV file into its corresponding SQL table (in the order of category, subcategory,contacts, campaign)
- Verify that each table has the correct data by running a SELECT statement for each from project2_campaignquery.sql

   
