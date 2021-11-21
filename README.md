# Pewlett-Hackard-Analysis
## Analysis Overview
The purpose of the analysis is to help provide information on the number of employees retiring per title and identify the number of employees eligible for the mentorship. The information will help management prepare for a huge influx of job openings. In order to complete the tasks at hand several queries in pgAdmin-PostgresSQL were performed to achieve the results. 

## Results
* In order to complete the analysis an ERD was created to visualize the relationship between the data sources and used to facilitate the purpose of this analysis.

  <img width="542" alt="Screen Shot 2021-11-20 at 11 40 00 PM" src="https://user-images.githubusercontent.com/91230916/142749828-8bdda233-8d92-4be4-a82f-b257b1b9e2f6.png">

* In the first analysis deliverable a retirement titles table was created to hold all the titles of current employees with the most recent title of each employee who were born between January 1, 1952, and December 31, 1955. The results came back that 133,776 employees will be retiring; however the results had duplicates.  In order, to remove the duplicates, the DISTINCT ON function was used to get a more informative dataset. The results without the duplicates were put into a unique titles table. The results show there are 90,398 employees retiring. 

  ![Screen Shot 2021-11-20 at 11 49 26 PM](https://user-images.githubusercontent.com/91230916/142750003-513905a8-e09e-4e33-b75f-2121af088247.png)

* In order to know how many employees retiring per titles, the COUNT function was used to generate the number of employees per title. After executing the code, it was found that there is a large number of employees holding senior titles (57,668/90,398=64) with around 64% of the staff to retire. 

  ![Screen Shot 2021-11-20 at 11 52 09 PM](https://user-images.githubusercontent.com/91230916/142750049-304f7b1d-3c96-4a20-92a1-87d62ac104a3.png)
  
* Below is a list of candidates that is eligible to become members of the mentorship program. 

  ![Screen Shot 2021-11-21 at 12 03 28 AM](https://user-images.githubusercontent.com/91230916/142750267-c5208837-d137-428e-aad1-d6c28ed4b490.png)

## Summary 
Currently at Pewlett Hackard, 64% of their employees are getting ready for retirement or being redirected to their mentorship initiatives, which will mean that they are likely going to need an extensive hiring process in the upcoming years. Since a significant amount of future retirees hold Senior positions the mentorship program should focus on those roles because extensive expertise will be leaving the company.

## Resources 
Data Sources: departments.csv, dept_emp.csv, dept_manager.csv, employees.csv, salaries.csv, titles.csv

Software: SQL, PostgreSQL, pgAdmin
