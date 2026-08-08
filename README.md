# Pizza-Sales-Analysis

## Pizza Sales Analysis Overview
This report presents a comprehensive analysis of my husband's money 
market investment with AXA Mansard from 2019 to 2024, based on the provided dataset. 
The primary objective of this analysis is to track deposits, liquidations, and profits 
generated from the money market investment. By examining these financial activities, 
this report aims to provide clearer insights into investment performance and offer strategic 
recommendations on optimizing returns by minimizing withdrawals or liquidations.

## Table of Content
- overview
- data processing
- data cleaning
- pivot table
- analysis

## Tools Used
- Microsoft Excel: Microsoft Excel: This was used for initial data loading and cleaning,
transforming the raw dataset into a structured format suitable for analysis.
- PivotTable: for analysis and visualization

## Dataset Overview
columns: pizza_id order_id	pizza_name_id	quantity	
order_date	order_time	unit_price	total_price	pizza_size	
pizza_category	pizza_ingredients	pizza_name


## Data Source
  This dataset was gotten from kaggle. dataset link
  below is the screenshot of the raw dataset

## Data Cleaning and Preparation

- ### Duplicating the Dataset
Before making any changes to the dataset, a duplicate copy was created.
This was done to preserve the original dataset and provide a backup in
case any cleaning or transformation resulted in unintended changes.

- ### Data Filtering and Duplicate Check
The Excel Filter function was activated to make it easier to
inspect, analyze individual columns and check for duplicates.

- ### Formatting the Date Column
The date column was formatted into a consistent date format
to ensure that all dates were correctly recognized by Excel.

- ### Extracting the Day of the Week:
The day of the week was extracted from the date column using the Excel TEXT function.

### Formula:
```excel
=TEXT(E2, "DDD")
```
- Weekday and Weekend Categorization
The order dates were further categorized into Weekday and Weekend.

### Formula:
```
=IF(WEEKDAY(E2,2)>=6,"Weekend","Weekday")
```
- ### Categorizing Orders by Time of Day
The order time was categorized into different periods of the day.

### Formula:
```
=IFS(
HOUR(H2)>=20,"Night-time",
HOUR(H2)>=16,"Evening",
HOUR(H2)>=12,"Afternoon",
HOUR(H2)<12,"Morning")
```
- ### Currency Formatting
The Unit Price and Total Price columns were converted to currency format.
to ensures that monetary values are displayed consistently and are easily understood.

- ### Cleaning the Pizza Ingredients Column
The Pizza Ingredients column was also cleaned to improve consistency and readability.
The cleaning process involved correcting inconsistencies such as spellings

- ### Converting the Dataset into an Excel Table
After completing the cleaning process, the dataset was converted into an Excel Table.

screenshot of the cleaned dataset

<img width="1343" height="644" alt="image" src="https://github.com/user-attachments/assets/445fb84f-093d-41a9-8904-54a935bc43df" />
<img width="1363" height="648" alt="image" src="https://github.com/user-attachments/assets/b8ad82c7-7753-4da0-b51e-b541b45113ca" />

## Skills Demonstrated
- Data cleaning   - Data preprocessing
- Microsoft Excel  - Excel formulas
- Data transformation  - Duplicate detection
- Date and time manipulation  - Data categorization
- Data formatting  - Excel Tables
- PivotTables  - Data analysis
- Data visualization  - Dashboard development
- Business insight generation

## Data Analysis and Visualization
