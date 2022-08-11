
#                                                                           Portfolio

---

# [Employment and Estimated Salary in the Data Science Field](/sample_page)

---
---

The field of data has been rapidly changing in recent years.
Job titles such as Data Analyst, Data Scientist, and Data Engineer may represent synonymous or completely different roles at various companies. I wanted to look at job listings for these three job titles and compare salary, skills etc. 

### Approach and Summary
The goal of this project is to pull data from Glassdoor (Kaggle source: https://www.kaggle.com/datasets/andrewmvd/data-analyst-jobs) and compare Data Analyst, Data Scientist and Data Engineer job listings in terms of salary, job skills and job locations. I used RStudio for the data analysis and PowerBI for data visualization. I utilized basic regression models to determine how salary changes with the change in title, skills, location etc.  

---
### Data and Data Cleaning
After getting the data from Kaggle, I removed any data that didn't fall under the 3 main job titles. After this, I created dummy variables for a list of 16 popular data science skills on whether or not they were included in the job description of the listing. Other data cleaning occurred as well including removing null values, duplicates and irrelevant columns. Below, is the distribution of salaries for the 3 job titles. 

<img src="images/Boxplots.PNG?raw=true" width=500/>

There are different skills associated with each of the job titles. SQL tends to be common across all three job titles and Python is extremely common for Data Scientists and Data Engineers. Excel was mentioned mostly in job listings for Data Analysts but is likely expected for Data Engineer and Data Scientist roles. 

<img src="images/BarChartforSkills.PNG?raw=true" width=1000/>

---
### Models and Conclusions

Below is the summary of the final regression model for the project. The salary fluctuated mainly due to job title and location of the job listing after being normalized based on cost of living. The highest paying job title is Data Scientist followed by Data Engineer and then Data Analyst. Based on cost of living, the best bang for your buck when looking for a data job would be to live in Texas or Illinois. California and New York actually had a lower average salary after the cost of living adjustment. 

<img src="images/FinalModel.PNG?raw=true"/>

Since none of the skills were significant in the model, I ran an additional one that only focused on skills and company size afterwards. I found that having Python in your skillset led to an increase in salary especially in the Data Analyst job title. Machine Learning being listed in the Job Description also led to an increase in salary. 

<img src="images/SkillsModel.PNG?raw=true"/>
---


---




---
<p style="font-size:11px">Page template forked from <a href="https://github.com/evanca/quick-portfolio">evanca</a></p>
<!-- Remove above link if you don't want to attibute -->
