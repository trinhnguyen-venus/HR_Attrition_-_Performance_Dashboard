# 📊 HR Attrition & Performance Analysis Dashboard

## 1. Project Context
This project simulates a real-world HR analytics case for an HR Manager, focusing on employee attrition, performance, and career progression.

The objective is to help HR leaders:

- Understand where attrition is happening
- Identify patterns across workload, satisfaction, income, and experience
- Support data-informed people decisions, not just reporting metrics

The focus is on business-relevant questions, analytical reasoning, and decision support.

<<<<<<< HEAD
## 2. Business Questions
The dashboard is designed to answer the following questions an HR Manager would typically ask:
=======

>>>>>>> a9a6ffb54e90f867e02f0e34a4aea8e8cb33c1c

1. Which departments and job roles have the highest attrition risk?
2. What are the key drivers of employee turnover?
3. How do workload, compensation, and job satisfaction relate to attrition?
4. Are there inequalities or patterns in income and performance across demographics?
5. How does career progression (promotion) differ by age group?

## 3. Key Metrics Tracked

- Headcount
- Turnover Rate
- Promotion Rate
- Average Work Years
- Average Age
- Average Job Satisfaction

## 4. Analytical Approach
The analysis follows a driver-based framework, not descriptive reporting:

- Segment attrition by department, job role, overtime, income level, and satisfaction
- Compare income and performance across gender
- Analyze career progression patterns using promotion rates by age group
- Validate findings across multiple dimensions to avoid single-metric bias

## 5. Key Insights
### 5.1 Attrition is driven by workload and satisfaction

- Employees not working overtime account for a larger share of total turnover compared to those working overtime.
- This suggests that overtime alone is not the main driver of attrition.
- Other factors such as role type, engagement, or career expectations may play a more significant role.

![Insert image](Images/Turnover_Rate_vs_Overtime.png)

### 5.2 Higher job satisfaction groups represent a larger portion of turnover

- Employees with job satisfaction levels 3 and 4 make up a higher share of attrition compared to levels 1 and 2.
- This indicates that turnover does not only come from dissatisfied employees.
- Possible explanations include:
- Employees with acceptable satisfaction still leave for better opportunities
- External market factors rather than internal dissatisfaction

![Insert image](Images/Turnover_Rate_vs_Job_Satisfaction.png)

### 5.3 Sales roles are attrition hotspots

- Sales roles appear frequently among the top job roles by turnover rate.
- This pattern suggests structural challenges such as:
  - Performance pressure
  - Variable income
  - Workload intensity

![Insert image](Images/Top_Job_Roles_by_Turnover_Rate.png)
![Insert image](Images/Turnover_Rate_by_Department.png)

### 5.4 Compensation differs by role, while performance remains comparable

- Managerial and research leadership roles have significantly higher average income.
- Income differences exist between genders, while average performance ratings are similar.
- This highlights the need to review compensation fairness separately from performance outcomes.

![Insert image](Images/Avg_Monthly_Income_by_Job_Role.png)
![Insert image](Images/Gender_Income_&_Performance_Comparison.png)

### 5.4 Promotion rate shows a clear downward trend with age

- Promotion rate decreases gradually across age groups:
  - Under 30: highest promotion rate
  - 30–40 and 40–50: moderate decline
  - 50+: lowest promotion rate
- This indicates that career progression opportunities become more limited as employees grow older, which may affect long-term engagement.

![Insert image](Images/Promotion_Rate_by_Age_Group.png)


## 6. Business Recommendations

Based on the analysis:

1. Investigate non-overtime employee turnover to understand underlying drivers beyond workload.
2. Conduct stay interviews even with moderately satisfied employees to capture external push factors.
3. Review Sales role structure, including targets, incentives, and workload balance.
4. Regularly assess pay equity, separating compensation review from performance evaluation.
5. Develop alternative career paths for senior employees beyond traditional promotions.

## 7. Intended Stakeholders

- HR Managers
- HR Business Partners
- People & Workforce Analytics Teams

## Author
**Trinh Nguyen**  

📧 Contact: ng.trinh3023@gmail.com

📍 GitHub: [https://trinhnguyen-venus.github.io/](https://trinhnguyen-venus.github.io/)
