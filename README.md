# Data Cleaning, Analysis, and Visualization Project Guide

## Introduction
I want to express my gratitude to Luke Barousse for providing the dataset, which serves as the foundation for this data cleaning, analysis, and visualization project downloaded from Kaggle.
![Στιγμιότυπο οθόνης 2024-02-05 103052](https://github.com/st9ho3/Data_Science_Job_Posts_Dashboard/assets/148724871/9a6b8e78-5bf3-475d-a8c2-7bd216ff0ce0)

## Data Cleaning

### Initial Cleaning
To begin, I'll conduct an initial assessment of the data, focusing on preparing it for analysis. Several columns will be removed:
- `job_id`
- `thumbnail`
- `posted_at`
- `schedule_type` (limited exploration due to the project's focus on skills-centric analysis)
- `salary` (broken down into different columns)
- `commute_time`
- `search_term` (limited to data analyst roles)
- `search_location` (limited to the US)
- `salary_pay`
- `index`

### Salary Structure Investigation
There appears to be an anomaly in the salary structure, specifically with yearly salaries having an additional 'zero' in their format, resulting in values appearing ten times higher than intended. A filter will be applied to the `salary_rate` column to further investigate and address this issue.

### Data Refinement
I've established a structured table to facilitate subsequent work, including the creation of a `degree` column, adjustments to the `work_from_home` column using an IF function, and standardization of salaries for comparability.

## Skills Extraction and Categorization

### Skills Cleaning
Utilizing MID and FIND functions, each skill is individually processed and split into distinct columns. Additionally, IF and SEARCH functions are employed to categorize job titles into four core roles: Data Analyst, Business Analyst, Data Scientist, and Data Engineer.

### Pivot Tables for Skill Frequency
For a comprehensive understanding, pivot tables are generated to display the frequency of each skill in relation to the identified job titles.

### Skill Summary and Ranking
A summarized table of skills is presented, accompanied by assigned ranks, ensuring focus on the top six relevant skills. The detailed functions and formulas are outlined in the 'Functions README.'

## Additional Analysis

### Metrics Pivot Tables
To conclude, pivot tables are utilized to capture and analyze various metrics beyond skills, providing a comprehensive overview of the dataset.

## Project Focus
While the `schedule_type` column was briefly explored, the project primarily aims to create an interactive dashboard centered around skills. The dashboard will showcase Excel skills and hands-on visualizations, offering users an engaging and informative experience.
