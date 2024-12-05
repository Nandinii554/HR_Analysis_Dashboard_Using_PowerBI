# HR Analytics Dashboard using PowerBI
This dashboard provides an in-depth analysis of HR workforce data, focusing on metrics such as headcount, salary, leave balance, and role-specific trends. It is designed to assist HR teams in monitoring workforce growth, analyzing compensation trends, and improving employee management strategies.

## Key Objectives:
- Understand workforce composition: Analyze headcount, gender distribution, and job-specific metrics.
- Monitor employee benefits: Evaluate leave balances and identify trends in leave utilization.
- Assess salary distribution: Study average, minimum, and maximum salary variations across roles.
- Facilitate decision-making: Provide actionable insights to improve workforce planning and management.

## **Data Source:** <br>
Platform: Kaggle <br>
Dataset: HR Workforce Analytics dataset containing 161 rows and 9 columns, including metrics such as job titles, salaries, leave balances, and joining dates.<br>

## **Data Transformation (Power Query):**<br>
Data was imported and cleaned using Power BI's Power Query Editor.<br>
Key transformations included:
- Removing null values and duplicates.<br>
- Formatting columns (e.g., dates for joining, numerical values for salaries and leave balances).<br>
- Creating a calculated column for leave balances exceeding 20 days.<br>

## **DAX Measures:**

- Headcount: Count of unique employee IDs.<br>
- Formula: Headcount = COUNT(HR_data[Emp ID])<br>
- Average Salary: Average salary of employees.<br>
- Formula: Avg Salary = AVERAGE(HR_data[Salary])<br>
- Average Leave Balance: Average leave days remaining.<br>
- Formula: Avg Leave Bal = AVERAGE(HR_data[Leave Balance])<br>
- Employees with Leave > 20 Days: Count of employees exceeding the threshold.<br>
- Formula: LBL over 20 days = COUNTROWS(FILTER(HR_data, HR_data[Leave Balance] > 20))

## Visualizations:
![image](https://github.com/user-attachments/assets/0d5b3320-7940-4c22-aaa4-8944e4152dc4)

- Key Metrics Panel:
Displays headcount, average salary, average leave balance, and count of employees with leave balances over 20 days.
- Cumulative Headcount by Date of Join:
Line chart showing workforce growth over the years.
- Headcount by Job Title:
Bar chart highlighting the distribution of employees across roles.
- Leave Balance by Job Title:
Bar chart comparing average leave balances and the number of employees exceeding 20 days.
- Education, Salary, and Qualification Analysis:
Scatter plot showing the relationship between qualifications and salaries.
- Salary Metrics Table:
Tabular view of job-specific metrics including average, minimum, and maximum salaries.

## Insights:
- The workforce has grown steadily, with a significant increase between 2018 and 2022.

![image](https://github.com/user-attachments/assets/5070d3d2-65a6-4a33-ad52-b8cf90f43b71)

- Research Scientists and Product Managers have the highest average salaries, while Quality Control roles have the lowest.

![image](https://github.com/user-attachments/assets/157e4be1-f23e-4a44-a351-f463b41b3e1d)

- Employees with higher qualifications tend to earn higher salaries.

![image](https://github.com/user-attachments/assets/c326838e-ad09-4f9c-ac58-e9e9ee1edf00)

- Roles like Research Scientist and Marketing Specialist show balanced leave utilization, whereas others have higher leave balances exceeding 20 days. 
 
## Suggestions:
- Focus on optimizing leave policies for roles with excessive leave balances to improve productivity.
- Reassess salary structures for roles with significant salary disparities.
- Leverage workforce growth data to plan for hiring trends and resource allocation.
- Introduce training programs for roles with low headcount but critical importance, such as Research Analysts.

## Conclusion: 
The HR Data Analysis Dashboard provides valuable insights into workforce dynamics, salary trends, and employee benefits. By leveraging this tool, HR teams can make data-driven decisions to enhance workforce management and overall organizational performance. Future iterations of the dashboard could include metrics for employee performance and attrition rates for a more comprehensive analysis.


