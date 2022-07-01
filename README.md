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
- Data Source : wikipedia.movies.json, movies_metadata.csv, ratings.csv (Csv file could not be upload because they are too big)

# Results #
## an ETL Function to Read Three Data Files ##
To Extract the three data files (wiki, kaggle, movielens). MovieLens is a website run by the GroupLens research group at the University of Minnesota. The Kaggle dataset pulls from the MovieLens dataset of over 20 million reviews and contains a metadata file with details about the movies from The Movie Database.<br>

The following depicts the wiki_movies_df DataFrame:<br>
![Movie_DataFrame](/Image/Wiki_Movies.png) <br>

The following depicts the kaggle_metadata DataFrame: <br>
![MataData](/Image/kaggle_metadata.png) <br>

The following depicts the ratings DataFrame: <br>
![Ratings](/Image/Rating.png) <br>

##  Extract and Transform the Wikipedia Data ##
Filtering out bad data is important, in order to get good clean data and a cleaned Wikipedia data is converted to a Pandas DataFrame for clear view.<br>
The following depicts the columns from wiki_movies_df DataFrame to a list:<br>
![wiki_movie](/Image/to_list.png) <br>
<br><br>

## Extract and Transform the Kaggle data ##
The extraction and transformation of the Kaggle metadata using the ETL function and performe the merging of Wikipedia and Kaggle DataFrames. <br>
![wiki_movie](/Image/Wiki_Movies.png)<br>
<br><br>

## The Movie Database ##
The Movie DataFrame consist of the movies table and ratings table in the SQL database, by adding elapsed time to the database.
The following depicts the movies table in SQL database.<br>
![movies_query](/resources/movies_query.png)<br>
The following depicts the ratings table in SQL database.<br>
![ratings_query](/resources/ratings_query.png)<br>
<br><br>
