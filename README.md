# Pewlett-Hackard-Analysis

## Overview

The purpose of this analysis is to help prepare Bobby’s manager for the “silver tsunami” as many current employees reach retirement age. The following tasks are to be completed: 

1. Determine the number of retiring employees per title.
2. Identify employees who are eligible to participate in a mentorship program.

## Results

***Deliverable 1: The Number of Retiring Employees by Title***
Using the ERD created in this module as a reference, create a Retirement Titles table that holds all the titles of employees who were born between January 1, 1952 and December 31, 1955. Because some employees may have multiple titles in the database—for example, due to promotions—we’ll need to use the DISTINCT ON statement to create a table that contains the most recent title of each employee. Then, use the COUNT() function to create a table that has the number of retirement-age employees by most recent job title. Finally, because we want to include only current employees in our analysis, be sure to exclude those employees who have already left the company. In order to conclude the aforementioned items, the following processes were undertaken:

1. What are the data relationships between tables needed to create this deliverable?
  - Looking at the entity relationship diagram (ERD) below, we were able to determine the relationships between the "employees" and "dept_employees" tables through the primary key (emp_no). 

ERD:

![ERD](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/ERD.png)


2. How will we script the queries in order to create the following tables: "retirement_titles", "unique_titles", and "retiring_titles"?
  - After the relationships between the initial tables became understood, the following three queries were scripted in order to generate the aforementioned tables, respectively:

Deliverable 1:

![Deliverable_1](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/deliverable1.png)

The following are the results of each query, respectively:

Query 1:

![Query_1](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/Query1.png)

Query 2:

![Query_2](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/Query2.png)

Query 3:

![Query_3](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/Query3.png)


***Deliverable 2: The Employees Eligible for the Mentorship Program***
Using the ERD you created in this module as a reference and your knowledge of SQL queries, create a mentorship-eligibility table that holds the current employees who were born between January 1, 1965 and December 31, 1965.

1. What are the data relationships between tables needed to create this deliverable?
  - Looking at the entity relationship diagram (ERD) above from the first deliverable, we were able to determine the relationships between the "employees",  "dept_employees", and "titles" tables through the primary key (emp_no).

2. How will we script the queries in order to create the "mentorship_eligibilty" table?
  - After the relationships between the three tables became understood, the following was scripted in order to generate the aforementioned table:

Deliverable 2:

![Deliverable_2](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/deliverable2.png)

Results:

![Results](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/Query4.png)


## Summary

To summarize, the following questions were asked and the subsequent additional queries were scripted in order to provide more insight into the upcoming "silver tsunami.":

1. How many roles will need to be filled as the "silver tsunami" begins to make an impact?
    - 72,458 roles will need to be filled.
2. Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
    - There are 240,124 current employees. Of those employees, 167,666 are not retirement eligible. With only 1549 qualified retirement-ready employees available to mentor, each mentor would need to oversee 108 employees. This does not seem feasibile and it is my opinion that there not enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees.

Current Employees:

![current_emp](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/Query5.png)
