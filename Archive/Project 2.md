Topic: ETL
Related to: [[Jupyter Lab]],  [[Programming timeline]]
Hashtags: #Python #Pandas #SQL 
*created: June 25, 2023*
*last modified: `=this.file.mtime`*

---
# Instructions
The instructions for this mini project are divided into the following subsections:

### 1) Create the Category and Subcategory DataFrames (30 points) 
### Jo Ann
	- Use str.split() method to separate category and subcategory into two columns.
	- Use .unique() method to create two new lists of category and subcategory titles.
	- Use list comprehension to add string text to pre-generated category and subcat id lists.
	- Create new DataFrames that combine the unique lists and these pre-generated id lists.
	- Use df.to_csv() method to write the category and subcategory DataFrames to a csv file.

### 2) Create the Campaign DataFrame (30 points)
### Timothy
	- Use df.copy() method to copy the crowdfunding DataFrame that has separate category and subcategory columns.
	- Use df.rename() method to rename certain columns.
	- Use .astype() method to convert goal and pledged columns to float. Might need to refresh kernal if having issues here.
	- Use datetime module and pd.to_datetime().dt.strftime() method to convert date values.
	- Drop columns by creating a new DataFrame using only selected columns from your current campaign DataFrame.
	- export as CSV

### 3) Create the Contacts DataFrame (15 points)
### Evan
	- Use regex to split out the grouped data.
	- Use str.split() method to separate first name and last name into two columns.
	- Use pd.DataFrame.drop() method to dleete the contact name column
	- Use df.loc method to reorder columns.
	- Export as CSV

### 4) Create the Crowdfunding Database (25 points)
### Evan
	- Use QuickDBD to pre-generate the SQL table schema.
	- Specify the data types, PKs and FKs.
	- Save as 'crowdfunding_db_schema.sql' and push to the github repo.
	- Create a new postgres db named 'crowdfunding_db'
	- Using the database schema, create the tables in the correct order to handle the foreign keys.    
	- Verify the table creation by running a `SELECT` statement for each table.
	- Import each CSV file into its corresponding SQL table.
	- Verify that each table has the correct data by running a `SELECT` statement for each.