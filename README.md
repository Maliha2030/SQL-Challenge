# SQL-Challenge

## Background

It’s been two weeks since I was hired as a new data engineer at Pewlett Hackard (a fictional company). My first major task is to do a research project about people whom the company employed during the 1980s and 1990s. All that remains of the employee database from that period are six CSV files.
For this project, I will design the tables to hold the data from the CSV files (data modeling), import the CSV files into a SQL database (data engineering), and then performing data analysis.


## Data Modeling - Entity Relationship Diagram

![ERD-sql_challenge](https://user-images.githubusercontent.com/113676942/211420581-8e70cd75-9f97-4e53-80bc-1aa097eeb1c6.png)

## Data Engineering - Primary and Foreign keys
### Primary keys:

'Title ID' is the primary key for the table 'Titles' (there is only one title id per title).
'Emp_no' in the table 'Employees' is the primary key. It is a unique ID for the table as there is only one employee number per employee.
'Dept_no' in table 'Departments' is unique/ the primary key with only one department number per department. 

### Foreign keys:

'Emp_no' in tables Dept_Emp, Salaries and Dept_Manager are foreign keys to the primary key 'Emp_no' in Employees.
'Dept_no' in tables Dept_Manager and Dept_Emp are foreign keys to the primary key 'dept_no' in the table Departments.

## Data Analysis

The following data analysis is carried out: 

a)List the employee number, last name, first name, sex, and salary of each employee.

b)List the first name, last name, and hire date for the employees who were hired in 1986.

c)List the manager of each department along with their department number, department name, employee number, last name, and first name.

d)List the department number for each employee along with that employee’s employee number, last name, first name, and department name.

e)List first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.

f)List each employee in the Sales department, including their employee number, last name, and first name.

g)List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.

h)List the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name).

