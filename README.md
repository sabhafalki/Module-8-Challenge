# Module-8-Challenge  Movies-ETL
# Overview of Project #
The purpose of this Project is to develop an algorithm to perdicte which low baget movie release will be the most popular, in order to buy the relevant streaming rights. Amazing Prime company had organised Hackathon event to collaborate with local teams to analyse the data, for the hackathon the teams have to gather data from both Wikipedia and Kaggle, combine them, and save them into a SQL database so that they have clean dataset by ELT process. Furthermore, create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. 

The analysis consisted of the following:
1. Extract the Wikipedia and Kaggle data from their respective files.
2. Transform the datasets by cleaning them up and joining them together.
3. Load the cleaned dataset into a SQL database.

# Resources #

- Extract : ETL_function_test.ipynb
- Transform : ETL_clean_wiki_movies.ipynb & ETL_clean_kaggle_data.ipynb <br>
- Load : ETL_create_database.ipynb <br>
- Languages : Python, SQL <br>
- Tools : Jupyter Notebook, JSON, Pandas, NumPy, sqlalchemy, psycopg2 <br>
- Data Source : wikipedia.movies.json, movies_metadata.csv, ratings.csv 

# Results #
## an ETL Function to Read Three Data Files ##
To Extract the three data files (wiki, kaggle, movielens).MovieLens is a website run by the GroupLens research group at the University of Minnesota.The Kaggle dataset pulls from the MovieLens dataset of over 20 million reviews and contains a metadata file with details about the movies from The Movie Database.<br>

![DBD](/Pewlett-Hackard-Analysis/Image/EmployeeDB.png)

##  Extract and Transform the Wikipedia Data ##
Filtering out bad data is important, in order to get good clean data and a cleaned Wikipedia data is converted to a Pandas DataFrame for clear view.<br>
![retirement_titles](/Pewlett-Hackard-Analysis/Image/retirement_titles.png) <br>

![unique_titles](/Pewlett-Hackard-Analysis/Image/unique_titles.png) <br>

![retiring_titles](/Pewlett-Hackard-Analysis/Image/retiring_titles.png)
<br><br>

## Extract and Transform the Kaggle data ##
The extraction and transformation of the Kaggle metadata using the ETL function and performe the merging of Wikipedia and Kaggle DataFrames. <br>
![mentorship_eligibility](/Pewlett-Hackard-Analysis/Image/mentorship_eligibility.png)
<br><br>

## The Movie Database ##
The Movie DataFrame consist of the movies table and ratings table in the SQL database, by adding elapsed time to the database.

