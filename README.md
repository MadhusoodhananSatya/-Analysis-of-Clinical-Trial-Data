# Analysis of Clinical Trial Data Using Spark SQL

## Overview
This project focuses on analyzing clinical trial data using Spark SQL. The primary goal was to clean, process, and explore key aspects of the dataset, such as study types, conditions, and trial durations. The analysis provided valuable insights into clinical trials, helping build a foundation for further research.

## Objective
The main objective is to gain insights from clinical trial data through cleaning, processing, and exploratory data analysis using Spark SQL.

## Key Features
-   **Data Cleaning**: Handled missing values in critical columns like 'Study Type', 'Conditions', and 'Study Status'. Also addressed multi-condition fields by splitting them for individual analysis.
-   **Exploratory Data Analysis (EDA)**: Investigated study types and conditions to understand the distribution and patterns within the dataset.
-   **Key Analysis**:
    -   Identified the most frequent study types and medical conditions.
    -   Calculated the average duration of clinical trials.
    -   Analyzed trends in diabetes-related clinical trials over time.
-   **Data Preparation**: Converted the loaded DataFrame into a temporary view (`clinical_trials`) to facilitate SQL queries.
-   **Null Value Checking**: Implemented SQL queries to identify and count NULL values in important columns, ensuring data quality.
-   **Unique Value Identification**: Explored unique values in categorical columns like 'Study Status' to understand data diversity.

## Technologies Used
-   **Apache Spark**: For distributed data processing and analysis.
-   **Spark SQL**: Used for querying and manipulating the clinical trial dataset.
-   **PySpark**: Python API for Spark, utilized for loading data and DataFrame operations within a Databricks environment.
-   **Databricks**: The environment where the Jupyter Notebook was developed and executed.

## Implementation Steps
1.  **Checking File Location**: Verified the presence of the `Clinicaltrial_16012025.csv` dataset in the `/FileStore/tables/` directory.
2.  **Creating the DataFrame**: Loaded the `Clinicaltrial_16012025.csv` file into a Spark DataFrame, inferring schema and handling headers and special characters.
3.  **Converting to Temporary View**: Converted the DataFrame into a temporary Spark SQL view named `clinical_trials` to enable SQL query execution.
4.  **Exploratory Data Analysis (EDA)**:
    -   Described the schema and columns of the `clinical_trials` view.
    -   Checked for and counted NULL values in key columns (`Study Type`, `Conditions`, `Study Status`, `Start Date`, `Completion Date`).
    -   Identified unique values in the `Study Status` column.
    -   Further analysis steps were performed as described in the "Key Analysis" section.

