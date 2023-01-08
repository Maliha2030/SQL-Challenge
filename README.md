# SQL-Challenge

**Background

It’s been two weeks since I was hired as a new data engineer at Pewlett Hackard (a fictional company). My first major task is to do a research project about people whom the company employed during the 1980s and 1990s. All that remains of the employee database from that period are six CSV files.
For this project, I will design the tables to hold the data from the CSV files (data modeling), import the CSV files into a SQL database (data engineering), and then performing data analysis.




**Data Engineering - Primary and Foreign keys
*Primary keys:

Title id is the primary key for Titles ie there is only one
 title id per title.

Emp_no in Employees is the unique ID for the table, ie there is only one employee number per employee. emp_no is the primary key for Employees.

Dept_no in Departments is primary key for Department as it is unique/ only one department number per department. 


*Foreign keys:

Emp_no in Dept_Emp is a foreign key i.e is primary key for a different table that is used in a new table. Emp_no is a forgeign key to the primary key emp_no in Employees i.e the values of emp_no in Dept_Emp match the values of the primary key emp_no in Employees.

Similarly Emp_no in Salaries, and Dept_Manager are foreign keys to the primary key emp_no in Employees.

Dept_no in table Dept_Manager and table Dept_Emp are foreign keys to the primary key dept_no in Departments as they match the values of dept_no in Departments.
