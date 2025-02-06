Employee Retention

Business Problem
Context
Client: HR department at a large software company.
 Initiative: "Proactive Retention" to predict which employees are likely to leave.
Goal: Use data to identify at-risk employees and intervene before they leave.
Scope: Focus on permanent (non-temp) employees.
Problems with Current Approach
Retroactive Process: HR learns about employee departures only after they leave, using exit interviews.
Main Issues:
Haphazard Insight: Quality of feedback depends on the interviewer’s skill.
No Systematic Aggregation: Can't aggregate insights from all employees who leave.
Not Proactive: Policy changes are driven by post-departure feedback.
1.3 Problem Statement
Task: HR hires data science consultants to build a proactive approach for retention.
Dataset: Provided by the business intelligence team with information on past employees and their status.
1.4 Business Objectives and Constraints
Deliverable: A trained machine learning model.
Interpretability: Model must be interpretable.
Output: Probabilities alongside predictions.
Constraints: No latency issues.

 Machine Learning Problem
2.1 Data Overview
Dataset: 14,249 records of past and present employees.
Departments: Data covers 12 departments.
Target Variable: Employee's status (Employed/Left).
Features:

Administrative Information:

department: Department the employee belongs to.
salary: Relative salary level in their department.
tenure: Number of years at the company.
recently_promoted: Whether the employee was promoted in the last 3 years.
Workload Information:

n_projects: Number of projects the employee is involved in.
avg_monthly_hrs: Average monthly working hours.
Mutual Evaluation Information:

satisfaction: Employee’s satisfaction with the company.
last_evaluation: Score from the most recent evaluation.
filed_complaint: Whether the employee filed a complaint in the last 3 years.
2.2 Mapping Business Problem to ML Problem
2.2.1 Type of Machine Learning Problem
Problem Type: Binary classification (predict if an employee is likely to leave or not).
2.2.2 Evaluation Metric (KPI)
Confusion Matrix: To measure correct and incorrect predictions.
ROC-AUC: Measures how well the model distinguishes between employees likely to leave and those who are not. The AUC score will help in model selection.

