
# Healthcare-Analysis-and-Insights
## Problem Statement
 - The healthcare industry generates vast amounts of data daily, providing valuable insights for healthcare providers and policymakers to improve patient care, allocate resources effectively, and manage healthcare costs. This project aims to analyze a comprehensive healthcare dataset comprising medical examinations, hospitalization details, and customer profiles to extract insights into patient health profiles, medical histories, and healthcare costs. By exploring relationships between various health metrics, identifying trends, and visualizing key patterns, we aim to deliver actionable insights to healthcare stakeholders for informed decision-making through rigorous data cleaning, transformation, exploration, and analysis.
## Dataset Discription
 - The given data set contain information of customers within different states. This data contains customer ID, date of birth, BMI, Age, statuses of BMI and HbA1c, State Id, Medical histories, charges, tiers etc.
## Data Preprocessing
## Data Cleaning
 - 1. checked the missing values marked with '?'in each column of the “Medical Examinations” Table and "Hospitalization Details" Table.
   2. Filled the missing values of ‘month’ with Sep and ‘year’ with its average rounded to the nearest integer
   3. The most frequently occurring values in 'smoker' is yes, whereas in hospital tier and city tier are tier3 and its      filled missing values accordingly
   4. The values that are missing in 'State ID' are replaced with "unknown".
   
## Data Transformation
- 1. Using "split text to columns", the customer names column split into three columns.
  2. Converted "Number of major surgeries" column in the "medical examination" table to numerical data using "find and replace", by changing the "no major surgeries" to 0".
  3. In both columns, I applied "PROPER" function.
  4. Created a new column named "Weight status" using the function "IF". The FUNCTION applied here is "IF(B2<18.5,"UNDERWEIGHT",IF(B2<24.99,"NORMAL",IF(B2<29.99,"OVERWEIGHT",IF(B2>30,"OBESITY"))))"
  5. Created a new column named "Diabetes status" using "IF" FUNCTION. The formula I applied here is
"IF(D2<5.7,"NORMAL",IF(D2<6.49,"PREDIABETES,IF(D2>6.5,"DIABETES")))
  6. Using CONCATENATE function, I merged the 'year' 'month' and 'date' columns into one column named "date of birth".
  7. Age calculated by using "2023-(year column).
  8. Changed charges column into currency format.
 ## Exploratory Data Analysis
  - This project focuses on analyzing Healthcare data. Identify patient trends, understand medical conditions and compare healthcare indicators through an interactive dashboard.
  -  It Analyze patient medical history. Compare cancer history among smokers and non smokers.
  -  Analyze major surgeries based on transplant history.
  -  Identify meaningful patterns in healthcare data.
  ## Key Analysis
   - Compared the distribution of cancer among smokers and nonsmokers to understand the relationship between smoking status and cancer history.
   - Compared the total number of major surgeries between patients with and without transplants.
   - Analyzed the difference in average HbA1C levels between patients with and without transplants.
   - Patients from different state Id distinguished during this analysis.
  ## Dashboard Overview
   - The total number of patients = 2333.
   - Out of 2333 patients, all of them are identified as smokers.
   - Average HbA1C Percentage is 6.58.

 This created as a part of My Data Analytic Learning Journey,
     Thank You.
