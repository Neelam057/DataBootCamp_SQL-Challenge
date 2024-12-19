# Pewlett Hackard Employee Data Analysis

## Overview

This project involves designing, importing, and analyzing employee data from the 1980s and 1990s at Pewlett Hackard (a fictional company). The company has six CSV files that hold the remaining records from the employee database from that period. The goal of this project is to perform data modeling, data engineering, and data analysis using SQL.

The steps covered in this project include:
1. **Data Modeling**: Designing the schema to hold the data from the CSV files and creating the necessary tables.
2. **Data Engineering**: Importing the CSV files into a SQL database and ensuring that the tables are correctly structured.
3. **Data Analysis**: Querying the database to answer specific business questions based on the employee data.


## **Project Structure**

The project directory structure is as follows:

```
EmployeeSQL/
├── data/
│   ├── departments.csv                      
│   ├── dept_emp.csv           
│   └── dept_manager.csv 
│   └── employees.csv
│   └── salaries.csv
│   └── titles.csv       
├── screenshots/                  
│   ├── Question1solution.png 
│   └── Question2solution.png
│   └── Question3solution.png 
│   └── Question4solution.png
│   └── Question5solution.png
│   └── Question6solution.png
│   └── Question7solution.png
│   └── Question8solution.png         
├── documentation.pdf
├── qdbd_erd.png
├── qdbd_schema.sql 
├── queries.sql 
├── schema.sql           
├── README.md                 

```

## Table Design and Schema

### Tables to be Created:
The following tables will be created to hold the data from the CSV files:

1. **employees**:
   - Contains employee details such as `emp_no`, `emp_title_id`, `birth_date`, `first_name`, `last_name`, `sex`, `hire_date`.
   
2. **departments**:
   - Contains department details, including `dept_no` and `dept_name`.
    
3. **salaries**:
   - Contains salary information for employees, including `emp_no` and `salary`
   
4. **titles**:
   - Contains job titles for employees, including `emp_no` and `title`.

5. **dept_emp**:
   - A relationship table that links employees to departments, containing `emp_no` and `dept_no`.

6. **dept_manager**:
   - A relationship table that links departments to employees, containing `dept_no` and `emp_no`.


### Entity Relationship Diagram (ERD)
An ERD (or table schemas) is created to represent the relationships between the tables.

## Data Import Process

### CSV File Import

The CSV files will be imported into the database using import/export in pgAdmin. The data will be imported into the corresponding tables:

1. **employees.csv**: Employee data will be imported into the `employees` table.
2. **departments.csv**: Department data will be imported into the `departments` table.
3. **salaries.csv**: Salary information will be imported into the `salaries` table.
4. **titles.csv**: Job titles will be imported into the `titles` table.
5. **dept_emp.csv**: Employee with their respective departments will be imported into the `dept_emp` table.
6. **dept_manager.csv**: Department with the respective department managers will be imported into the `dept_manager` table.


## Queries and Data Analysis

Once the data is imported, the SQL queries will be executed to answer the business questions provided in the requirements section. These queries will leverage SQL joins and groupings to provide the necessary insights.

## Conclusion

This project involves designing an efficient relational database schema, importing data into the database, and performing several analyses to answer specific business questions. Each phase of the project has been carefully planned, from data modeling to data engineering and data analysis. The results will provide valuable insights into the employee records of Pewlett Hackard from the 1980s and 1990s.
