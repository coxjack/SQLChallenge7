## Pewlett-Hackard Analysis
Challenge 7 for Butler Data Science

## 1. Overview of PH Analysis
### 
* The goal of this module is to assist a large company with their analysis of their employees, specifically focused on upcoming retirements. For this analysis we focused on current employees born between January 1, 1952 and December 31, 1955, this allowed us slice our employees to only those reaching retirement age in the near future. During our research we looked to answer the following questions
	- Who will be retiring?
	- How many positions will Pewlett-Hackard need to fill?
	- Which employees have the skills and experience to help younger employees transition to senior positions?

## 2. Results
### 
* Retiring Titles
	- The simplest of the tables in our analysis was looking what positions had the most employees that would be retiring in the near future. 
	- Senior level positions will be hit hard by upcoming retirements 
	- The engineering department is set to lose a total of ~35,000 employees. 
	- Luckily for PH only two managers are included in the retirement bracket. 

	  - Retiring Titles

![Retiring Titles](https://github.com/coxjack/SQLChallenge7/blob/main/additional%20supporting%20images/RT.png)

* Retirement Titles & Unique Titles
	- These two tables give us essentially the same data. The retirement_titles table includes all iterations of an employee while unique titles narrows it down to only an employee's most recent position. Since there is non-current duplicates in the retirement titles table -- it makes sense to focus our analysis on the unique_titles table.
	- Looking at the unique_titles table we are able to see that there are 72,458 potential retirees at Pewlett-Hackard. 

* Mentorship Eligibility
	- The final table in our analysis looks at current employees who were born between January 1, 1965 and December 31, 1965. These employees are not quite yet at retirement age but will be relatively soon. The idea is that these employees would be good candidates to act as mentors for younger employees moving into roles vacated by the retiring employees.
	- Looking at this table we are able to see that there are 1,549 potential mentors at Pewlett-Hackard. 

	  - Mentorship Eligibility

![ME](https://github.com/coxjack/SQLChallenge7/blob/main/additional%20supporting%20images/ME.png)
	
## 3. Summary
### 
* How many roles will need to be filled as the "silver tsunami" begins to make an impact?
	- From the select count query ran for the unique_titles table -- we can see that there are 72,458 potential retirees at Pewlett-Hackard.

	  - Total Potential Retirees

![Unique Titles](https://github.com/coxjack/SQLChallenge7/blob/main/additional%20supporting%20images/UT.png)

* Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
	- No, from the select count query ran for the mentorship_eligibility table -- we can see there are only 1,549 employees that fit the mentorship conditions. Every mentorship candidate would have to mentor ~46 employees in order to have a mentor for every retiring position. 


