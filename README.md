# LinkedIn Job Listings Web Scraping with Python

## Overview
This project demonstrates how to use Python with Selenium for web scraping job listings from LinkedIn. Specifically, it extracts job details for Data Scientist positions in Indonesia. The information scraped includes job title, company name, location, posting date, job description, seniority level, employment type, job function, and industry. The data is then saved to an Excel file for further analysis.

## Prerequisites

Before running the project, ensure you have the following installed:

- Python 3.x
- Chrome browser
- ChromeDriver (matching your Chrome browser version)
- Selenium library
- Pandas library
- OpenPyXL library (for writing to Excel)

## Objectives
1. **Web Scraping**: Extract job listing data from LinkedIn, including details such as job title, company, location, job level, and employment type.
2. **Data Cleaning**: Process and refine the data to ensure accuracy and usability by fixing inconsistencies and removing irrelevant entries.
3. **Analysis Preparation**: Organize and export the cleaned dataset for data analysis.

## Features
### Web Scraping
- Extracted job listings using XPATH to retrieve structured data fields.
- Managed challenges like empty fields and inconsistencies due to HTML structure.
- [View Web Scrapping Script.]([https://github.com/juwitardiyanti/SQL_personal_project/blob/main/northwind_sample_database/northwind.sql](https://github.com/juwitardiyanti/Linkedln-Web-Scrapping/blob/main/web-scrapping.ipynb])

### Data Cleaning
1. **Data Understanding and Cleansing**:
   - Identified data structure and field rules.
   - Checked data relevancy and field distributions.

2. **Location Parsing**:
   - Split the `location` field into `city`, `province`, and `country`.
   - Addressed varying formats in location data.

3. **Job Level and Type Fixes**:
   - Corrected misplaced values between `Level` and `Type` fields.
   - Ensured accurate definitions of job levels and employment types.

4. **Categorization and Filtering**:
   - Categorized job titles into "Data Scientist" or "Others" based on keywords.
   - Removed unrelated job listings for focused analysis.

5. **Column Selection**:
   - Retained only relevant columns: `date`, `company`, `title`, `location`, `city`, `province`, `level`, `type`, `function`, `industry`, and `title_category`.

## Dataset Overview
The final dataset includes the following columns:
- **date**: The posting date of the job listing.
- **company**: The company offering the job.
- **title**: The job title.
- **location**: The full location field as listed.
- **city**: The parsed city name.
- **province**: The parsed province name.
- **level**: The seniority level.
- **type**: Employment type.
- **function**: Job function or department.
- **industry**: General field of the company.
- **title_category**: Generalized job title category (e.g., Data Scientist, Others).

