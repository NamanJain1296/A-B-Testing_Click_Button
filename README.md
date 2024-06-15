# A-B-Testing_Click_Button
This repository contains a Python script designed to conduct a simulated A/B test, a widely used method in statistics and data science for comparing two versions of a single variable. This project serves as a practical example to demonstrate the process of A/B testing, providing an educational case study for data analysis and hypothesis testing.
![image](https://github.com/NamanJain1296/A-B-Testing_Click_Button/assets/113998224/3905e268-1e92-44fa-aa29-207fb4dffb8c)
<br/>
# 1. Simulating Click Data for A/B Testing
## Objective:
To simulate click data for an experimental group (exp) and a control group (con).

- Method (generating data similar to what we use in our case study)
- Utilizes numpy and pandas libraries to generate random binary click data (1 = click, 0 = no click).
- Creates two datasets: df_exp for the experimental group and df_con for the control group.
- Each group has 1000 samples with different click probabilities (0.5 for exp and 0.2 for con).
- Merges the data into a single DataFrame df for analysis.
  ![image](https://github.com/NamanJain1296/A-B-Testing_Click_Button/assets/113998224/16033806-b6e7-471a-89ef-b8050d862f63)
<br/>

# 2. Statistical Significance in A/B Testing
## Objective
To determine if the difference in click rates between the experimental and control groups is statistically significant.

## Method
Calculates total number of clicks (X_con, X_exp) and click probabilities (p_con_hat, p_exp_hat) for each group.
Computes a pooled click probability (p_pooled_hat) and pooled variance.
Calculates standard error (SE) to measure the precision of click probability estimates.
Performs a two-sample Z-test (calculates test statistic (Test_stat), critical value (Z_crit), and p-value).
Determines a confidence interval (CI) to estimate the true difference in click probabilities.
<br/>
# Application as a Case Study
## Scenario
A website is testing two different webpage designs to see which one results in higher user engagement, measured by clicks.

## Process
The exp group is shown the new webpage design, while the con group sees the original design.
The script simulates user interactions and calculates the click-through rate for each group.
Statistically analyzes the results to assess if the new design significantly improves user engagement.
<br/>
# Conclusion
## Findings
The script provides statistical evidence on whether the new design (experimental group) leads to a higher click rate compared to the control group.
![image](https://github.com/NamanJain1296/A-B-Testing_Click_Button/assets/113998224/363ec577-0052-4a34-a91d-7c2024637e40)
<br/>
# Decision Making
Decisions are made based on the p-value and confidence interval, determining the implementation of the new design across the website.
