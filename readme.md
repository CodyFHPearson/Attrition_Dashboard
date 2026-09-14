# IBM HR Attrition Analysis

## Project Summary

For this project, I assumed the role of an HR Data Analyst for IBM and was tasked with developing an interactive dashboard to analyze employee attrition across several workforce metrics. The dashboard allows stakeholders to evaluate key performance indicators relating to current and former employees, examine the relationship between career progression and attrition, and explore how employee survey responses relate to attrition.

In addition to developing the dashboard, I was provided with a series of business questions to investigate. Based on the results, I identified key insights and developed actionable recommendations intended to support employee-retention efforts.

For a more detailed explanation of the chart creation process, view the [full project documentation](attrition_dashboard_documentation.pdf).

## Disclaimer

This dashboard and its accompanying analysis use the fictional “IBM HR Analytics Employee Attrition & Performance” dataset obtained from Kaggle. This independent portfolio project is not affiliated with or endorsed by IBM. The project was completed solely to demonstrate my data-analysis and Tableau skills.

## Dashboard Purpose

The purpose of this dashboard is to provide stakeholders with an overview of employee attrition and the ability to investigate workforce factors that may be associated with employees leaving the organization. The Overview section presents company-wide attrition metrics, compares the average income and tenure of current and former employees, and shows differences in attrition and workforce size across departments.

The dashboard also allows stakeholders to examine how attrition relates to career progression, job level, employee survey responses, and job role. Interactive department and overtime filters, along with selectable career-progression and survey metrics, enable users to explore specific employee groups and identify areas that may warrant further investigation or targeted retention efforts.

## Dashboard Requirements

### General

- Allow dashboard results to be filtered by department and overtime status.
- Use consistent colors to identify attrition rates that are above or below the corresponding average.
- Display detailed subgroup results only when the group contains at least 30 employees or survey responses.
- Provide a legend explaining the dashboard’s colors, symbols, and workforce-size encoding.

### KPI Overview

- Display the number of current employees, number of former employees, and overall attrition rate.
- Compare the average monthly income and tenure of current and former employees.
- Compare workforce size and attrition rates across departments.

### Career-Progression Analysis

- Display attrition-rate trends for three career-progression metrics: Years at Company, Years in Current Role, and Years Since Last Promotion.
- Allow users to switch between the three career-progression metrics.
- Highlight areas of particularly high or low attrition as each career-progression metric relates to job level.
- Display workforce size to provide context for the attrition rates shown.

### Survey-Response Analysis

- Display attrition-rate trends for four employee survey measures: Environment Satisfaction, Job Satisfaction, Relationship Satisfaction, and Work-Life Balance.
- Allow users to switch between the four survey measures.
- Highlight areas of particularly high or low attrition across survey responses and job roles.
- Display the number of responses represented by each job-role result.

## Analytical Questions

The analysis was designed to answer the following questions:

1. **How is attrition distributed across the organization, and how do current and former employees compare?**
2. **How are employee tenure and job level associated with attrition?**
3. **Are workplace experiences associated with employees leaving?**

## Dashboard

### Video Demo

▶️ **[Watch the interactive dashboard walkthrough](https://youtu.be/NLbCEp6yoYQ)**

###  Dashboard Screenshots

![IBM HR Attrition Dashboard](attrition_dashboard.png)

![IBM HR Attrition Dashboard with filters displayed](Attrition_dashboard_filters.png)

## Insights

### 1. Overtime employees experienced substantially higher attrition

Employees working overtime had an attrition rate of 30.53%, compared with 10.44% among employees who did not work overtime. Higher attrition among overtime employees was also consistently observed when the workforce was broken down by tenure and Job Satisfaction responses. Among Job Level 1 employees with no completed years in their current role, overtime employees had a 75% attrition rate across a workforce of 40, while employees who did not work overtime had a 29% rate across a workforce of 96. Among employees with two years or less at the company, overtime employees had a 51% attrition rate across a workforce of 104, compared with 20% across 238 employees who did not work overtime. Overtime employees also had higher attrition across every adequately represented Years at Company group and every Job Satisfaction response category. Overall, overtime was consistently associated with elevated attrition throughout the dataset.

### 2. R&D combines the largest workforce with the lowest departmental attrition

Research and Development had the largest workforce but the lowest departmental attrition rate at 13.84%, compared with 19.05% in HR and 20.63% in Sales. Four comparatively low-attrition roles, Healthcare Representative, Manager, Manufacturing Director, and Research Director, had a combined attrition rate of 5.86%. This suggests that R&D’s job-role composition may contribute to its lower overall attrition rate.

### 3. Sales Representatives account for a disproportionate share of Sales attrition

Sales Representatives made up 18.8% of the Sales department’s workforce but accounted for 35.5% of its former employees. The role had an attrition rate of 39.6%, the highest of any job role in the organization. Sales Representatives also had the lowest average tenure, which was more than two years shorter than any other role. Among employees classified as Sales Representatives, 55% had worked at the company for two years or less and 98% held Job Level 1 positions. These findings indicate that attrition within the Sales department was disproportionately concentrated among early-tenure employees working in entry-level Sales Representative positions.

### 4. Early-tenure attrition is concentrated at Job Level 1

Attrition was highest among early-tenure employees at Job Level 1. Among employees with two years or less at the company, the attrition rate was 36.74% at Job Level 1 and 20.00% at Job Level 2. Job Level 1 continued to show elevated attrition among employees with more than two years at the company, recording a rate of 20.39%. It was the only job level above the company-wide attrition rate within this tenure group. These findings indicate that Job Level 1 employees experienced elevated attrition across tenure groups, with the highest rate occurring among those in their first two years with the organization.

### 5. Job Satisfaction produced the strongest survey pattern, but the evidence was not conclusive

Of the four survey measures examined, Job Satisfaction displayed the strongest negative linear relationship with attrition. Lower satisfaction responses were associated with higher attrition rates, and the model explained approximately 89% of the variation across the four aggregated response categories. However, the relationship was not statistically significant at the 5% level (p = .056). Given the small number of aggregated response categories, this finding should be interpreted as a notable descriptive pattern rather than conclusive statistical evidence.

## Recommendations

### Review overtime practices and workloads

Conduct a review of overtime usage to determine which roles require or rely on it most frequently and why. Employee feedback should be collected to assess whether overtime reflects temporary staffing needs, persistent workload imbalances, or employee preferences. The organization could then test workload adjustments or additional staffing within heavily affected groups and monitor whether attrition declines.

### Strengthen support for early-tenure employees at Job Level 1

Develop a structured retention program for Job Level 1 employees during their first two years with the organization. The program should include regular manager check-ins, clearly communicated advancement requirements, and access to development opportunities. Retention rates should be monitored at key points throughout the first two years to identify when additional support may be needed.

### Prioritize Sales Representatives for further investigation

Conduct interviews with current Sales Representatives and review exit feedback from former employees to identify the conditions contributing to the role’s 39.6% attrition rate. The investigation should examine factors such as workload, compensation, job expectations, and advancement opportunities. Based on the findings, the organization could introduce a targeted retention initiative and compare subsequent results with the role’s historical attrition rate.

### Continue investigating Job Satisfaction

Use periodic employee surveys to determine whether the observed relationship between Job Satisfaction and attrition persists as additional data are collected. Survey results should be reviewed alongside overtime status and employee tenure to help identify groups that may require attention. Because the current statistical evidence was not conclusive, further investigation should take place before attributing attrition to Job Satisfaction or implementing any broad organization-wide response.
