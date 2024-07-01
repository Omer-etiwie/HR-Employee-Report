# HR-Employee-Report

### Project Overview
---

This data analysis project aims to provide insights into the distribution performance  over the 10 years. By analyzing various aspects of the data, we need to make data-driven recommendations and gain a deeper understanding of the company's performance.

![Dashboard-1](https://github.com/Omer-etiwie/HR-Employee-Report/assets/171517937/821b4087-c283-43b1-9394-f8f71af2ec43)
![Dashboard-2](https://github.com/Omer-etiwie/HR-Employee-Report/assets/171517937/71f5cfdc-ffeb-4310-bb44-36cf627d66c5)


### Data Sources

HR Data: The primary dataset used for this analysis is the "Human Resources.csv" 

### Tools

- SQL Server - Data cleaning & Analysis
-  PowerBI - Creating reports

### Data Cleaning/Preparation

In the initial data preparation phase, we performed the following tasks:
1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formatting

### Exploratory Data Analysis

EDA involved exploring the sales data to answer key questions, such as:

- What is the gender distribution of employees in the company?
- What is the age distribution of employees in the company?
- Which department has the highest turnover rate?

  ![Ex-PIC](https://github.com/Omer-etiwie/HR-Employee-Report/assets/171517937/b3a9bfd9-83e0-491d-8ee9-2a54aa4c8b73)


### Data Analysis

Include some interesting code/features worked with
  
  ```sql
  select 
        case  
              when age >=21 and age <=24 then '21-24'
              when age >=25 and age <=34 then '25-34'
              when age >=35 and age <=44 then '35-44'
              when age >=45 and age <=54 then '45-54'
              when age >=55 and age <=64 then '55-64'
              else '65+'
       end as age_group,gender,
  count(*) as count
  from copyoftest
  where age >=21 and termdate = '0000-00-00'
  group by age_group,gender
  order by age_group,gender;
  ```

### Results/Findings

The analysis results are summarized as follows:
1. The male has the highest gender distribution in the company.
2. The age between 35/44 has the highest distribution in the company.






 
  






