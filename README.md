# Sleep Pattern Data Analytics

Author: Niranjan  
Date: 1 May 2025

---
# Business Problem
1.	Does being a clerical or a construction worker influence toptal sleep and work hours?
2.	How Do married indivisuals with young kids manage their lseep and relaxation time compared to those with without kids?
3.	Is there a wage gap in hourly earnings between self-employes vs labour union members vs salaried employees?
4.	What’s the impact of living in urban areas (SMSA) or the south on sleep duration and work hour ?
5.	Do indivisuals in good health report significant different work hours and sleep patterns than those in poorer health?

 ---

# Project Background


This project explores the sleep patterns of working individuals, focusing on how various factors such as work hours, income, health, gender, education, and family responsibilities impact sleep and leisure time. The objective was to identify key patterns that influence the quantity and quality of sleep and provide insights for personal well-being, work-life balance, and health-conscious decision-making.

Insights and recommendations are provided on the following key areas:


- **Work and Sleep Relationship**
- **Health and Lifestyle Impact**
- **Family and Demographic Influence**
- **Income, Occupation, and Time Use**

The Python notebooks used to inspect, clean, and analyze the data can be found here `Sleep_Data_Analytics_1.ipynb`and `Sleep_pattern_analysis_2.ipynb`.
An pdf of the complete documentation for the columns description can be found here ` `.
An executive presentation summarizing the results can be found here `Sleep Project Documentation.pdf`  
An interactive visualization dashboard will be added shortly 

---

# Data Structure & Initial Checks

The project's dataset, `sleep_data.csv`, was sourced from Kaggle and includes detailed information on working individuals across the United States.
The cleaned data set redy for visualization, `cleaned_sleep_data.csv`.
The primary data fields are as follows:

1.	**age**                               : Age in years.
2.	**clerical_worker**               : Yes if the individual is a clerical worker.
3.	**construction_Worker**   : Yes if the individual is a construction worker.
4.	**education**                 : Years of schooling
5.	**earns_1974**                  : Total earnings in 1974.
6.	**good_health**            : Yes if the individual is in good or excellent health.
7.	**labour_force**          : Yes if the individual is in the labor force.
8.	**awake_time**         : Sleep time (including nap) minus working time in Hours
9.	**free_time**              : Relaxation and leisure time minus working time.
10.	**smsa_area**             : Yes if the individual lives in a Standard Metropolitan Statistical Area (SMSA).
11.	**male**                            : Yes if the individual is male.
12.	**marital_status**        : Yes if the individual is married.
13.	**protestant**                : Yes if the individual is Protestant.
14.	**relax_time**            : Total relaxation and leisure time, including personal activities.
15.	**self_employed**                : Yes if the individual is self-employed.
16.	**sleep**                       : sleep at night per week in hours
17.	**total_sleep_week**          : sleep, including naps, per week in hours.
18.	**south**                        : yes if the individual lives in the South.
19.	**spouse_income**         : Spousal wage income.
20.	**spouse_works**                 : yes if the spouse works.
21.	**totwrk_hr**             : Hours worked per week.
22.	**labour_union**          : Yes if the individual belongs to a labor union.
23.	**young_kid**                 : Yes if children under 3 years old are present.
24.	**years_married**        : Years married.
25.	**hourly_wage**                : Hourly wage.
26.	**nap_per_week_hour** : total_sleep_week  -  sleep (total nap hours in a week)
27.	**total_work_time**         : main_job_wrork_time + Worked_second 


---

# Executive Summary

### Overview of Findings

The analysis revealed a strong inverse relationship between work hours and sleep time—those working longer hours tend to sleep less. Married individuals and those with young children generally sleep less and have reduced leisure time. Health plays a significant role—individuals in good health sleep more on average. Income levels also influence leisure time, while education correlates positively with wages but not with sleep. Self-employed individuals experience more flexible sleep and leisure hours, and occupation types show varied time-use patterns.

---

# Insights Deep Dive

### Sleep Time Distribution

* Most individuals sleep between 40 and 60 hours per week.
* Very few participants report sleeping less than 35 or more than 70 hours weekly, showing a centralized pattern with few outliers.
![Sleep Distribution](images/Sleep_distribution.png)

### Relationship Between Sleep and Work Hours

* Individuals working more than 40 hours per week sleep significantly less.
* A clear negative trend is observed—each additional hour of work reduces sleep time.
* Some individuals manage balance, but the overall trend supports a trade-off between labor and rest.
![Sleep vs Work Hours](images/Sleep_vs_WorkHours.png)

### Health Impact on Sleep

* Individuals reporting good health consistently sleep more than those in poor health.
* The sleep gap between good and poor health categories ranges from 4 to 7 hours weekly.
* This pattern underlines the connection between health and rest.
![Health vs Sleep](images/Sleep_by_Health_Status.png)

### Impact of Marital Status and Kids

* Married individuals sleep around 3 hours less weekly compared to unmarried counterparts.
* Presence of young kids further reduces average sleep time, indicating added family responsibilities.
* This highlights time constraints in family-oriented households.
![Sleep by Family](images/Sleep_by_Married_and_Kids.png)

### Gender Differences in Sleep, Wage, and Work

* Males work more hours on average but also report slightly higher incomes.
* Females tend to have slightly higher sleep and leisure time, but lower wages.
* Gender-based role divisions are reflected in both time and income distribution.
![Gender vs Sleep](images/Gender_vs_Sleep_Wage_Work.png)

### Education and Income Trends

* Higher education levels correlate with higher income and hourly wages.
* However, individuals with higher education do not sleep more—possibly due to demanding roles.
* A trade-off between career progression and personal time is visible.
![Education vs Income and Sleep](images/Education_vs_Income_Sleep.png)

### Occupation Type and Sleep Patterns

* Clerical workers tend to have more sleep and leisure hours compared to construction workers.
* Construction roles are more labor-intensive, leading to reduced rest and recreation time.
* Job type influences daily time allocation beyond just wages.
![Occupation vs Sleep](images/Sleep_by_Occupation_Type.png)

---

# Recommendations

Based on the analysis above, the following actions are recommended:

* Encourage better work-life balance by limiting extreme work hours and promoting flexible scheduling.
* Prioritize health-focused initiatives in both personal and professional environments, as good health supports better sleep.
* Family-focused policies such as childcare support can improve rest opportunities for married individuals and parents.
* Education and upskilling are essential for income growth, but individuals should be mindful of time management to maintain well-being.
* Employers can consider job-type flexibility and rest provisions in high-effort roles like construction.

---

# Assumptions and Caveats

Several assumptions were made to address data limitations:

* Missing values were removed from the dataset; they accounted for less than 5% of the total entries.
* Binary fields (e.g., good_health, male, married) were treated as 1 = Yes, 0 = No.
* Occupation categories were treated as non-exclusive; an individual could fall into more than one group.
* No time-series data was involved; analysis is cross-sectional based on current responses only.

---

## 📬 Contact
For queries or collaborations:
- **Email**: [niranjan991100@gmail.com]
- **LinkedIn**: (https://www.linkedin.com/in/niranjan-k-a83517229/)
