# Pewlett-Hackard-Analysis

## Overview

The purpose of this analysis is to help prepare Bobby’s manager for the “silver tsunami” as many current employees reach retirement age. The following tasks are to be completed: 

1. Determine the number of retiring employees per title.
2. Identify employees who are eligible to participate in a mentorship program.

## Results

***Deliverable 1: The Number of Retiring Employees by Title***
Using the ERD created in this module as a reference, create a Retirement Titles table that holds all the titles of employees who were born between January 1, 1952 and December 31, 1955. Because some employees may have multiple titles in the database—for example, due to promotions—we’ll need to use the DISTINCT ON statement to create a table that contains the most recent title of each employee. Then, use the COUNT() function to create a table that has the number of retirement-age employees by most recent job title. Finally, because we want to include only current employees in our analysis, be sure to exclude those employees who have already left the company. In order to conclude the aforementioned items, the following processes were undertaken:

1. What are the data relationships between tables needed to create this deliverable?
  -Looking at the ERD

ERD:

![ERD](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/ERD.png)

Deliverable 1:

![Deliverable_1](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/deliverable1.png)


***Deliverable 2: The Employees Eligible for the Mentorship Program***
Using the ERD you created in this module as a reference and your knowledge of SQL queries, create a mentorship-eligibility table that holds the current employees who were born between January 1, 1965 and December 31, 1965.

Deliverable 2:

![Deliverable_2](https://raw.githubusercontent.com/krismbah/Pewlett-Hackard-Analysis/main/deliverable2.png)


## Summary

To summarize, the following were asked and the subsequent additional queries were scripted in order to provide more insight into the upcoming "silver tsunami.":

1. How many roles will need to be filled as the "silver tsunami" begins to make an impact?
2. Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
