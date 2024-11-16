# Job-Satisfaction-Attrition-PowerBI
![Screenshot 2024-11-14 232056](https://github.com/user-attachments/assets/76cdfabd-39d2-49e9-aa33-f08759c3b9e3)


# Job Satisfaction & Attrition: Key Insights for Workforce Retention

This project focuses on creating an interactive Power BI dashboard to analyze employee attrition, identify key drivers, and provide actionable insights to improve workforce retention strategies. Below is a detailed breakdown of the steps taken to transform raw employee data into a dynamic and insightful dashboard.

---

## 1. Data Gathering
- Imported raw employee data from a CSV file into Power BI.
- Data included details such as employee demographics, job satisfaction ratings, attrition status, and departmental information.
- Utilized Power Query Editor to clean and process the data for further analysis.

---

## 2. Data Cleaning
Data cleaning was a crucial step to ensure data accuracy and consistency. The following tasks were performed:
- **Removing Empty Columns**: Removed irrelevant or empty columns to streamline the dataset.
- **Removing Duplicates**: Identified and eliminated duplicate records to maintain accuracy.
- **Error Handling**: Standardized inconsistent values and corrected formatting issues.
- **Data Type Detection**: Ensured each column had the correct data type (e.g., numeric, text, date).

These cleaning tasks prepared the dataset for deeper analysis.

---

## 3. Data Processing
### Attrition Analysis
- Created a new column, `AttritionCount`, using the conditional column feature.  
  - If an employee left the organization (attrition status = "Yes"), the value was set to `1`. Otherwise, it was set to `0`.

### Attrition Rate Calculation
- Created a DAX (Data Analysis Expressions) measure for the Attrition Rate:
- Attrition Rate = SUM([AttritionCount]) / SUM([EmployeeCount])
- Formatted this measure as a percentage to track employee turnover.

These measures formed the foundation for visualizations and KPIs in the dashboard.

---

## 4. Data Analysis and Visualization
The core phase of the project involved creating visualizations and KPIs to uncover key insights. Key visualizations included:
- **Bar Charts**: Compared attrition rates across departments, job roles, and gender.
- **Pie and Donut Charts**: Represented the distribution of employees by categories such as education field, business travel, and gender.
- **Matrix Tables**: Displayed detailed job satisfaction ratings across employee groups.
- **Key Performance Indicators (KPIs)**: Showed metrics like total employee count, average salary, and average age.
- **Clustered Bar Charts**: Highlighted departmental attrition trends.

Each visualization was crafted to provide actionable insights into different aspects of employee retention.

---

## Key Insights and Findings
The dashboard revealed several critical insights into employee attrition:
1. **Total Employees**: The organization currently employs 1,470 individuals, indicating growth.
2. **Attrition Analysis**:
 - 237 employees left the organization (150 males and 87 females).
 - Male employees exhibited a higher attrition rate.
3. **Departmental Attrition**:  
 - The Research and Development Department had the highest attrition rate at **56.13%**, suggesting targeted interventions are needed.
4. **Education Field Impact**:  
 - Employees from the Life Sciences field had the highest attrition rate, highlighting the need for retention strategies in this area.
5. **Job Role Impact**:  
 - Sales department employees exhibited the highest attrition rate, requiring focused efforts to enhance engagement and retention.
6. **Education-wise Attrition**:  
 - High School graduates had the highest attrition rate at **18.24%**.
7. **Age Group Attrition**:  
 - Employees aged 25-34 years had the highest attrition count, with 112 employees leaving the company.

---

## Key Features of the Dashboard
### Calculated Fields
- **Attrition Rate**: Tracks turnover percentage.
- **Active Employees**: Monitors workforce size over time.

### Visualizations
- **Matrix Table**: Displays job satisfaction ratings across different segments.
- **Donut and Pie Charts**: Represents gender distribution and departmental attrition rates.
- **KPI Indicators**: Highlights key metrics like total employee count, average salary, and job satisfaction.
- **Filters and Slicers**: Allow users to explore data by education fields, departments, and job satisfaction levels.

---

## Conclusion
The Power BI dashboard serves as a comprehensive tool for HR professionals, offering deep insights into employee attrition trends and the underlying causes of turnover. By visualizing attrition across departments, roles, and demographics, HR teams can:
- Make informed decisions.
- Develop targeted retention strategies.
- Proactively address attrition challenges.

With data-driven insights, organizations can significantly improve employee retention and foster a more engaged workforce.
