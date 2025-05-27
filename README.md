# hiring-data-2021

This repository contains two Snowflake SQL queries developed for analyze employee hiring trends in 2021 using Snowflake SQL.

## Files

- `query_1.sql`: Aggregates the number of employees hired per department and job title for each quarter of 2021.
- `query_2.sql`: Identifies departments that hired more employees than the average across all departments in 2021.

## Query Details

### Query 1 – Hires by Quarter per Department and Job

**Purpose**:  
To show how many employees were hired in each quarter of 2021, grouped by department and job title.

**Logic**:
- Joins the `HIRED_EMPLOYEES` table with `DEPARTMENTS` and `JOBS` for descriptive fields.
- Filters records from 2021.
- Groups results by department and job.
- Outputs the count of hires per quarter (Q1–Q4).

### Query 2 – Departments Hiring Above Average

**Purpose**:  
To identify departments that hired more than the average number of employees in 2021.

**Logic**:
- Aggregates the number of hires per department.
- Calculates the average hires across all departments.
- Filters for departments with hire counts above the average.
