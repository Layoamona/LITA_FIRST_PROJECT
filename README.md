# LITA_CLASS_DOCUMENTATION
This is where I documented my First project while learning Data Analysis with  Incubator Hub
## Introduction to Data Analysis
Data analysis is the processof inspecting, cleaning, transforming, modeling and visualizing and analysising data to dicover useful information, draw conclusions and support decision making.
## Data Structure

There are three different ways to structure data namely:

- Structured data (usually in tabular format)
- Semi-structured data (not in tabular form but it can be transformed into table. It is usually in Jason and Xml format)
- Unstructured data ( comes in media files)
## Life Cycle of Data Analysis

The data analysis process, often known referred to as data analysis cyle, consits of several steps that guide analysts from collecting raw data to making informed decisions. Each stage is crucial for tuning data into actionable insights. These cycle include:

- Data collection( also know as data ingestion)
- Transformation (also known as data cleansing)
- Modeling
- Visualization
- Analysis
- Presentation

## Tools Used
- Microsoft Excel  
  1. For Data Cleaning
  2. For Analysis
  3. For Visualiation
     
- SQL - Strutured Query Language for Quering Dta
-  GitHub for Portfolio Building
-  Power BI
  1. For Data Cleaning
  2. For Visualization
  3. Interractive Dashboard

  In order to have an indept understanding of the above stated tools, we worked on some projects.

  ## Project Overview
  The project helps to collect and analyze sales data from different various companies, markests and stores. It is s a comprehensive project designed to manage and analyze employee records, salary details, and payment information efficiently. This system leverages both SQL for robust database management, Microsoft Excel and Power Bi for data cleaning, organization, and advanced analysis. The project demonstrates the integration of these tools to create a seamless workflow for handling HR and payroll data. The primary source of data used here is an open source data that can be freely downloaded from an open source online such as Kaggle or FRED or any other repository sites, with additional datasets created by LITA to support specific project needs and analysis.

  ## Table of Content 
  - Excel Components
    1. Data cleaning and organization
    2. Data recovery and formatting
    3. Summary metrics calculations
    4. Pivot tables for analysis
  - SQL Components
    1. Database creation
    2. Table definition
    3. Data insertion
    4. Data manipulation operations
    5. Queries and analysis
    6. Data importation and analysis
  - Power BI
    1. Data cleaning
    2. Data visualization

  ## Excel Components
  ### Data Cleaning and Organization
   Raw payroll data was imported into Excel, where it was meticulously cleaned and organized:
   
   Separating Data into Columns: Ensured each data point (e.g., Names, Department, Salary) was placed in its respective column.
   
   Removing Unnecessary Rows: Eliminated rows containing summaries or irrelevant information to maintain data integrity.

### Uncleaned Salary Data
  
![Uncleaned Salary data](https://github.com/user-attachments/assets/e22f1e5c-88b7-45f1-ad23-3b275caca099)


### Cleaned Salary Data
![Cleaned Structured Salary Data](https://github.com/user-attachments/assets/b9aa717d-7620-457a-b53e-858c2e110ccf)

### Data Recovery and Formatting
 We were able to make use of some text functions functions in Excel like : LEFT, MID, RIGHT. These functions are used to manipulate and extract specific portions of text from a cell. Here is how each one works:

- LEFT Function: Extracts a specified number of characters from the beginning (left side) of a text string.

Syntax: =LEFT(text, num_chars)

- RIGHT Function: Extracts a specified number of characters from the end (right side) of a text string.

 Syntax: =RIGHT(text, num_chars)

- MID Function: Extracts characters from the middle of a text string, based on a specified starting position and number of characters.


 Syntax: =MID(text, start_num, num_chars)

 
![Lost Records](https://github.com/user-attachments/assets/1682d5e4-a6f1-4154-9412-e773783f4124)




### Data Extraction and Retrieval Based on some Instruction Given and with the Aid of the Text Functions

![Data Extraction and Retrieval](https://github.com/user-attachments/assets/6bc444e7-4baf-49da-a1de-0b8eef77cfcb)


### Pivot Table
This is a data summarizing tool. We used a pivot table to gain insights into revenue trends and sales performance across regions, and to calculate key metrics, such as total revenue by region and stores.


![pivot table](https://github.com/user-attachments/assets/05214cb2-5b4b-416b-b659-c109ce63ed4f)

## SQL Components

  1. We created a database in which we inputed some of our queries.
```SQL
CREATE DATABASE LITA_DB
```

    
 2. Data Insertion
``` SQL
CREATE TABLE Employee (
staffid varchar (255) not null,
FirstName varchar (255) NOT NULL,
SecondName varchar (255),
Gender varchar (10),
Date_of_Birth date,
HireDate datetime,
primary key (staffid)
)

Select staffid, firstname from Employee

```

3. Data Manipulation Operations
    
   They help modify database. Example of manipulative function include; 'insert', 'update' and 'delete'
   
``` SQL
insert into Employee (staffid, firstname, secondname, gender,Date_of_Birth, hiredate)
values ( 'AB401', 'ayan', 'olakun', 'female', '1992-08-22', '2018-02-09'),
( 'AB212', 'okorie', 'mercy', 'female','1988-10-09', '2018-10-09'),
( 'AB223', 'joshua', 'chukwuemeka', 'male','1980-10-09', '2022-02-09'),
( 'AB234', 'sanni', 'ibrahim', 'male','1958-10-09', '2019-09-23'),
( 'AB254', 'mercy', 'olanipekun', 'female','1982-10-09', '2020-02-09'),
( 'AB249', 'johnson', 'mercy', 'female','1982-10-09', '2019-12-09'),
( 'AB298', 'ayomide', 'halleluyah', 'female', '1982-10-09','2018-07-11'),
( 'AB260', 'deborah', 'justin', 'female','1982-10-09', '2018-02-09'),
( 'AB281', 'wale', 'olanipekun', 'male','1982-10-09', '2018-02-09')

------ Create salary table -------
CREATE TABLE Salary (
salary_id int identity (1,1)not null,
Staffid varchar (255),
firstname varchar (255),
lastname varchar (255),
department nvarchar(max),
salary decimal (10, 3)
)

select * from salary

------ insert employee salaries --------
insert into salary (staffid, FirstName, lastname, Department, Salary)
values ( 'AB401', 'ayan', 'olakun', 'Information Tech.', 45000.45),
( 'AB212', 'okorie', 'mercy','Account',500000.99999),
( 'AB223', 'joshua', 'chukwuemeka', 'Human Resources',100560.9339999),
( 'AB234', 'sanni', 'ibrahim', 'Sales and Marketing',845688.99),
( 'AB254', 'mercy', 'olanipekun', 'Account',8889.999999),
( 'AB249', 'johnson', 'mercy', 'Information Tech.',234000.90909090),
( 'AB298', 'ayomide', 'halleluyah', 'Logistics', 678000.991999),
( 'AB260', 'deborah', 'justin', 'Logistics',900099.00697969),
( 'AB281', 'wale', 'olanipekun', 'Information Tech',873093.2344)

----delete sql command--

delete from employee

where staffid  = 'ab281'

```

4. Queries and Analysis

   We made use of Excel functions like MAX, SUM, COUNT to determine the highest, lowest, fourth-highest, and third-lowest salaries.

```SQL

SELECT SUM(Salary) AS TOTALSALARY FROM Salary

SELECT AVG(Salary) AS AVERAGESALARY FROM Salary

SELECT COUNT(Staffid) AS EmployeeCount FROM EMPLOYEE

SELECT COUNT(Staffid) AS NumberOfEmployee FROM Salary

Update Salary
set salary = 7056999.9994
where Staffid = 'AB401'

```

5. Data Importation and Analysis
   We imported data from our excel into our SQL Studio and did some analysis.Steps to import data;

   1. Navigate to the database you want to import data into
   2. right click and click on tasks after which, you navigate to import flat file if file has been converted to Comma Separated Value File (csv)
   3. Select the location where your file was saved and import your data.
   4. Begin analysis.
  
## Power BI
  Power BI is a business intelligence and data visualization tool developed by Microsoft that allows users to connect, transform, visualize, and share data insights in an interactive way. It is  commonly used for creating dynamic reports and dashboards that make data more accessible and actionable for businesses and organizations.

### Uses of Power BI 

  1. 
