# Questions to Help You Practice for Your Data Science Interview

Divided in two main categories:
1. Coding Questions (in this article SQL, Python)
2. Non-Coding Questions (System Design, Probability, Statistics, Modeling, Technical, Product).

### CODING -> SQL
#### Question 1: Monthly Percentage Difference
Given a table of purchases by date, calculate the month-over-month percentage change in revenue. The output should include the year-month date (YYYY-MM) and percentage change, rounded to the 2nd decimal point, and sorted from the beginning of the year to the end of the year. The percentage change column will be populated from the 2nd month forward and can be calculated as ((this month’s revenue — last month’s revenue) / last month’s revenue)*100.

#### Question 2: Premium vs Freemium
Find the total number of downloads for paying and non-paying users by date. Include only records where non-paying customers have more downloads than paying customers. The output should be sorted by earliest date first and contain 3 columns date, non-paying downloads, paying downloads.

#### Question 3: Marketing Campaign Success
You have a table of in-app purchases by user. Users that make their first in-app purchase are placed in a marketing campaign where they see call-to-actions for more in-app purchases. Find the number of users that made additional in-app purchases due to the success of the marketing campaign.
The marketing campaign doesn’t start until one day after the initial in-app purchase so users that only made one or multiple purchases on the first day do not count, nor do we count users that over time purchase only the products they purchased on the first day.

#### Question 4: Total Wine Revenue
You have a dataset of wines. Find the total revenue made by each winery and variety that has at least 90 points. Each wine in the winery, variety pair should be at least 90 points in order for that pair to be considered in the calculation.
Output the winery and variety along with the corresponding total revenue. Order records by the winery in ascending order and total revenue in descending order.

#### Question 5: Class Performance
You are given a table containing assignment scores of students in a class. Write a query that identifies the largest difference in total score of all assignments. Output just the difference in total score (sum of all 3 assignments) between a student with the highest score and a student with the lowest score.

### CODING -> PYTHON
#### Question 6: Median Salary
Find the median employee salary of each department. Output the department name along with the corresponding salary rounded to the nearest whole dollar.

#### Question 7: Average Salaries
Compare each employee’s salary with the average salary of the corresponding department. Output the department, first name, and salary of employees along with the average salary of that department.

#### Question 8: Employee with Bonuses
Find employees whose bonus is less than $150. Output the first name along with the corresponding bonus.

### NON CODING -> SYSTEM DESIGN
#### Question 9: Restaurant Recommendation
How would you build a ‘restaurants you may like’ recommender system on the news feed?

#### Question 10: Python Dictionary to Store Data
When would I use a Python dictionary to store data, instead of another data structure?

#### Question 11: Build a Recommendation System
Can you walk us through how you would build a recommendation system?

### NON CODING -> Probability
#### Question 12: Four People in an Elevator
There are four people in an elevator that is about to make four stops on four different floors of the building. What is the probability that each person gets off on a different floor?

#### Question 13: Pick 2 Queens
Probability of choosing 2 queens out of a deck of card?

### NON CODING -> Statistics
#### Question 14: Central Limit Theorem
Explain central limit theorem.

#### Question 15: Assessing Multicollinearity
What are different techniques to assess multicollinearity?

#### Question 16: Precision and Recall
Provide formulas for precision and recall.

### NON CODING -> Modeling
#### Question 17: Few instances Labeled
What techniques can be used to train a classifier using a large dataset in which only a small proportion of instances are labeled?

#### Question 18: Features Correlation
What happen if two features correlates in a linear regression?

### NON CODING -> Technical
#### Question 19: Database Normalization
List and shortly explain the steps of the database normalization process.

#### Question 20: N-Gram
What is a n-gram?

### NON CODING -> Product
#### Question 21: Customer Engagement and Disengagement
How do you measure customer engagement and disengagement?

#### Question 22: Click on Search result
You notice that the number of users that clicked on a search result about a Facebook Event increased 10% week-over-week. What steps would you take to investigate the reason behind the change? How do you decide if the change has a good or bad impact on the business?




