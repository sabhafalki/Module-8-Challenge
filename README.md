# Module-8-Challenge  Movies-ETL
# Overview of Project #
The purpose of this Project is to develop an algorithm to perdicte which low baget movie release with be popular, so that they can buy the streaming rights. Amazing Prime company had organised Hackathon event to collaborate with local teams to analyse the data, for the hackathon the teams have to gather data from both Wikipedia and Kaggle, combine them, and save them into a SQL database so that they have clean dataset by ELT process. 

The analysis consisted of the following:
1. Extract the Wikipedia and Kaggle data from their respective files.
2. Transform the datasets by cleaning them up and joining them together.
3. Load the cleaned dataset into a SQL database.

# Resources #

- Extract - ETL_function_test.ipynb
- Transform - ETL_clean_wiki_movies.ipynb & ETL_clean_kaggle_data.ipynb <br>
- Load - ETL_create_database.ipynb <br>
- Languages: Python, SQL <br>
- Tools: Jupyter Notebook, JSON, Pandas, NumPy, sqlalchemy, psycopg2 <br>
- Data Source(s): wikipedia.movies.json, movies_metadata.csv, ratings.csv 

# Results #
## The ER Data Diagram ##
The following depicts the DB Schema. <br>
![DBD](/Pewlett-Hackard-Analysis/Image/EmployeeDB.png)

##  The Number of Retiring Employees by Title ##
The following tables mentions the retiring employees by title, on the basis of their birth dates (i.e. born between 1952 and 1955). <br>
![retirement_titles](/Pewlett-Hackard-Analysis/Image/retirement_titles.png) <br>

The following table is filtering the above for unique values only. <br>
![unique_titles](/Pewlett-Hackard-Analysis/Image/unique_titles.png) <br>

The following table counts the number of employees based on their titles. <br>
![retiring_titles](/Pewlett-Hackard-Analysis/Image/retiring_titles.png)
<br><br>

## The Employees Eligible for the Mentorship Program ##
The following table depicts the Employees' who are eligible for the mentorship program. <br>
![mentorship_eligibility](/Pewlett-Hackard-Analysis/Image/mentorship_eligibility.png)
<br><br>

# Conclusion #
## Summary ##
From our analysis, we were able to conclude that the following:
1. After analyzing the number of retiring employees by their titles, we were able to conclude that more than 60% of their employees are getting ready for retirement. The count of employees expected to retire is 90,398.
2. We were also able to conclude that the senior staff also had senior designations, which made sense.
3. We also realized that the highest number of Employees leaving were Senior Engineers and the Senior Staff. 
4. There appears to be a high numebr of employees retiring, hence the organization needs to backfill. 

## Further Analysis ##
The following table provides a summary of the number of employees eligible for the mentorship program based on their designation. 
It is evident from the table below, that the Senior Staff and Egineers were amonghst the hightest to be eligible for the mentroship program. <br>
![unique_titles](/Pewlett-Hackard-Analysis/Image/mentorship_emp.png) <br>

The following table provides a summary of the number of employees eligible for the mentorship program based on their department. 
Based on the table below, we can conclude that the Development and Production Department had the hightest retirement rates. <br>
![unique_titles](/Pewlett-Hackard-Analysis/Image/retirement_departments.png) <br>
