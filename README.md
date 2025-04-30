# Sleep Pattern Data Analytics

Author: Niranjan  
Date: 1 May 2025

---

# Project Background


This project explores the sleep patterns of working individuals, focusing on how various factors such as work hours, income, health, gender, education, and family responsibilities impact sleep and leisure time. The objective was to identify key patterns that influence the quantity and quality of sleep and provide insights for personal well-being, work-life balance, and health-conscious decision-making.

Insights and recommendations are provided on the following key areas:


- **Work and Sleep Relationship**
- **Health and Lifestyle Impact**
- **Family and Demographic Influence**
- **Income, Occupation, and Time Use**

The Python notebooks used to inspect, clean, and analyze the data can be found here `Sleep_Data_Analytics.ipynb`.  
An executive presentation summarizing the results can be found here `Sleep Project Documentation.pdf`  
An interactive visualization dashboard will be added shortly 

---

# Data Structure & Initial Checks

The project's dataset, `sleep_data.csv`, was sourced from Kaggle and includes detailed information on working individuals across the United States.
The cleaned data set redy for visualization, `cleaned_sleep_data.csv`.
The primary data fields are as follows:

- **sleep**: Weekly hours spent sleeping (excluding naps)
- **slpnaps**: Weekly hours spent sleeping including naps
- **totwrk_hr**: Weekly working hours
- **totleisure_hr**: Weekly leisure hours
- **hourly_wage**: Wage earned per hour
- **income**: Total income
- **male**: Gender indicator
- **married**: Marital status
- **youngkids**: Presence of children under 6 years
- **education**: Education level
- **experience**: Years of work experience
- **selfemployed**: Employment type indicator
- **good_health**: Health condition indicator
- **inlf**: Labor force participation
- **smsa**, **south**: Regional classification
- **clerical**, **construction_Worker**: Job category indicators

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
