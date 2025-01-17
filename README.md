# HR Analytics Project: Atliq Technologies (April to June FY2022)

## Project Overview
This project focuses on analyzing the attendance data of Atliq Technologies employees for April, May, and June 2022. By cleaning and transforming the data, the goal is to provide actionable insights that help the HR team monitor employee presence, working preferences, and leave trends to improve planning and decision-making.

## Problem Statement
Atliq Technologies operates on a hybrid working model, with some employees working from the office while others work remotely. The HR team needs insights into attendance data to address key concerns, including:

- The percentage of employee presence over the last three months.
- Work preferences (work-from-home vs. in-office attendance).
- The frequency of sick leaves taken by employees.

## Tools and Technologies
- **Power BI**: For creating an interactive dashboard and visualizing insights.
- **Power Query**: For efficient Extract, Transform, and Load (ETL) processes.
- **DAX**: For creating calculated fields, metrics, and KPIs.

## Data Cleaning Process
To streamline data cleaning and transformation, the following steps were taken in **Power Query Editor**:

### 1. Created a Template for Data Standardization
**Why?** Since data from multiple months had inconsistent structures, creating a standardized template allowed uniform processing of all sheets.

**Steps:**
- Loaded one month's attendance data (e.g., April 2022) as a base to design the template.
- Standardized column names, ensured headers were correctly promoted, and filtered out irrelevant data.
- Used the "Unpivot Other Columns" function to convert wide-format data into a long-format table for better usability.
- Ensured the template structure aligned with the expected final dataset format.

### 2. Created Parameters for Flexibility
**Why?** Parameters made the cleaning process adaptable for different months without manual intervention for each dataset.

**Steps:**
- Defined a parameter for the month (e.g., "April 2022," "May 2022") to dynamically select data from corresponding sheets.
- Used the parameter to automate the query, ensuring only the relevant sheet was processed when switching months.

### 3. Built a Custom Function for Reusability
**Why?** To eliminate redundancy and apply the same cleaning logic across multiple months' datasets.

**Steps:**
- Created a custom function in Power Query for transforming the data (e.g., renaming columns, unpivoting, changing data types, and removing errors).
- Applied this function to all monthly sheets (April, May, and June) using the template as a reference.
- This ensured consistent processing and saved significant time.

### 4. Combined and Consolidated Data
- After processing each sheet using the custom function, merged the cleaned data from April, May, and June into a single consolidated table.
- Validated the data by comparing it to the "Attendance Key" reference sheet, ensuring all codes were correctly interpreted.

## Key Features of the Data Cleaning Process
- **Dynamic Template Design**: Standardized the dataset for each month to avoid manual adjustments.
- **Parameterization**: Enabled the use of flexible parameters for seamless month-to-month switching.
- **Reusable Functions**: Built a single transformation logic that was consistently applied across all sheets, increasing efficiency and accuracy.

## Insights Derived
The cleaned and consolidated data allowed for the creation of KPIs and visualizations, including:

- **Employee Presence Trends**: Monthly and individual attendance rates.
- **Work Preferences**: Work-from-home vs. in-office ratios.
- **Leave Analysis**: Frequency and types of leaves (e.g., Sick Leave, Work-Off).

## Screenshots


## Results and Impact
- **Streamlined Workflow**: Automated the cleaning process for all months, reducing manual effort.
- **Enhanced Decision-Making**: Provided clear insights into attendance patterns and trends.
- **Efficiency**: Saved the HR team significant time in generating reports and analyzing data.

## Acknowledgments
Special thanks to **Dhaval Patel** and **Hemanand Vadivel** for the guided project and Codebasics for providing a detailed walkthrough.

## Project Resources
- **Link to Project Playlist**: [YouTube Playlist](https://www.youtube.com/playlist?list=PLeo1K3hjS3uuVQccZa7yFwK3ltoGQOWbM)
- **Interactive Dashboard**: [NovyPro Link](https://www.novypro.com/project/atliq-hr-analytics)
