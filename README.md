
This research project concerns creating a database of people whom Pewlett Hackard employed during the 1980s and 1990s. All that remains of the employee database from that period are six CSV files.

For this project, I designed the tables to hold the data from the CSV files, imported the CSV files into a SQL database, and then answered questions about the data.


This project was completed according to the following workflow: 

Data Modeling
Inspect the CSV files, and then sketch an ERD of the tables. 

Data Engineering
Use the provided information to create a table schema for each of the six CSV files. Be sure to do the following:

Remember to specify the data types, primary keys, foreign keys, and other constraints.

For the primary keys, verify that the column is unique. Otherwise, create a composite keyLinks to an external site., which takes two primary keys to uniquely identify a row.

Be sure to create the tables in the correct order to handle the foreign keys.

Import each CSV file into its corresponding SQL table.

Data Analysis

List the employee number, last name, first name, sex, and salary of each employee.

List the first name, last name, and hire date for the employees who were hired in 1986.

List the manager of each department along with their department number, department name, employee number, last name, and first name.

List the department number for each employee along with that employee’s employee number, last name, first name, and department name.

List first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.

List each employee in the Sales department, including their employee number, last name, and first name.

List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.

List the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name).


from sqlalchemy import create_engine
engine = create_engine('postgresql://localhost:5432/<your_db_name>')
connection = engine.connect()


Create a histogram to visualize the employee salary ranges that were the most common.

Create a bar chart of average salary by title.


Create an image file of your ERD.

Create a .sql file of your table schemata.

Create a .sql file of your queries.

**Methods used:**

SQL

Jupyter Notebooks

ERD 

Primary Keys
