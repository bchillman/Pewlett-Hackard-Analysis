# Pewlett-Hackard-Analysis
## Overview
This analysis was done for the purpose of determining more information about how many employees in Pewlett-Hackard will be retiring soon. As initial analysis showed that there would be a large number of these retirees, it was deemed important to find out more information about this so-called "Silver Tsunami." The following queries were made:

1. A table with all employees born from 1952 to 1955, and their titles
2. The same table, but only including the employees' current titles
3. The number of retiring employees grouped by their title
3. A table with all employees born in 1965, as those employees are deemed the correct age for mentoring new employees.



## Resources
- Data Source: Pewlett-Hackard database
- Software: PostgreSQL 11.13, PGAdmin

## Pewlett-Hackard Analysis Results
The following results were taken from the analyses:

1. As there are 72,458 rows in the second table, we can expect that number of employees to be retiring soon.
2. There are a large number of employees with the titles "Senior Engineer" and "Senior Staff" so these higher level positions will need the most filling.
3. There are only 2 managers in the retirement age, so there will be very little turnover at that high-level position.
![retiring_titles](https://github.com/bchillman/Pewlett-Hackard-Analysis/blob/main/Data/retiring_titles.PNG)

(Points 2 and 3 can be referenced with this screenshot of the third table).

4. As there are 1,549 rows in the fourth table, we can expect that number of employees to be available to mentor.
 
## Pewlett-Hackard Analysis Summary
### Summary of Results
As the "Silver Tsunami" begins to take effect, and these employees begin to retire, there will eventually be over 70,000 retirements, which means that there will need to be over 70,000 hires, in addition to any promotions that take place. There are only 1,549 employees that fit the initial requirements for being eligible to mentor, however these requirements are somewhat restrictive, and may not be optimal for finding the best mentors. First, we only looked at employees who were born in 1965, which is strangely specific, and can be expanded. Second, looking at the birth date for eligibility to mentor doesn't seem ideal, as someone older could be new to the company. Instead we will inspect how long employees have been in the company. However, when the employees are ordered by the date at which they started in the department they are in, the newest employee start date was in August 2002. This either implies that the data is 20 years old, or nobody new has started in a department in the last 20 years. Either way, we will take our new mentors from a list that is filtered by employees who joined in 1992 (10 years experience), and were born in 1960 or later so as not to include employees retiring. This list can be found in the membership_eligibility file in the data folder, and includes  43,392 employees, a number much closer to the ~70,000 retirees. With these employees, each mentor would only have to mentor 2-3 new hires, with extra room to spare for some of these employees to leave or not be suitable to mentor. Next, we mwill check the titles of employees on this mentor listto ensure that tthere are sufficient mentors for each title.

