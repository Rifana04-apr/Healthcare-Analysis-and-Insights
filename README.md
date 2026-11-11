# Healthcare-Analysis-and-Insights
## Problem Statement
 - The healthcare industry generates vast amounts of data daily, providing valuable insights for healthcare providers and policymakers to improve patient care, allocate resources effectively, and manage healthcare costs. This project aims to analyze a comprehensive healthcare dataset comprising medical examinations, hospitalization details, and customer profiles to extract insights into patient health profiles, medical histories, and healthcare costs. By exploring relationships between various health metrics, identifying trends, and visualizing key patterns, we aim to deliver actionable insights to healthcare stakeholders for informed decision-making through rigorous data cleaning, transformation, exploration, and analysis.
## Dataset Discription
 - The given data set contain information of customers within different states. This data contains customer ID, date of birth, BMI, Age, statuses of BMI and HbA1c, State Id, Medical histories, charges, tiers etc.
## Data Preprocessing
 - 1. checked the missing values marked with '?'in each column of the “Medical Examinations” Table and "Hospitalization Details" Table.
   2. Filled the missing values of ‘month’ with Sep and ‘year’ with its average rounded to the nearest integer
   3. The most frequently occurring values in 'smoker' is yes, whereas in hospital tier and city tier are tier3 and its      filled missing values accordingly
   4. The values that are missing in 'State ID' are replaced with "unknown".
