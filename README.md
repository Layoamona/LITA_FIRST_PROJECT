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
