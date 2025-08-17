# 🎬 Movie Database Analysis (Serverless SQL with Jupyter Notebook)

<img src="https://github.com/Explore-AI/Pictures/blob/master/sql_tmdb.jpg?raw=true" width=80%/>

# 📖 Project Overview

This project explores the Movie Database (TMDB) using a serverless SQL approach within a Jupyter Notebook environment. 
The goal was to answer a series of analytical questions about movies, actors, genres, awards, and production companies by directly querying the database without deploying or managing a dedicated database server.

The project demonstrates skills in SQL querying, data analysis, database normalization concepts, and interactive exploration of structured datasets. 
It also highlights how a serverless workflow can streamline analytics for datasets stored locally or in cloud-managed services.

# ⚙️ Tools & Technologies Used

  - **Jupyter Notebook:** Interactive environment for running SQL queries alongside explanations, results, and visualizations.
  
  - **SQLAlchemy:** Python SQL toolkit used to connect to the SQLite TMDB database (`sqlite:///TMDB.db`) in a serverless fashion.
  
  - **ipython-sql** (`%load_ext sql`): Magic command extension that allows running SQL queries directly inside **Jupyter Notebook** cells.
  
  - **SQLite:** Lightweight, file-based relational database engine used as the backend (no dedicated server required).

  - **GitHub:** To publish the project as a portfolio, including SQL scripts, query results, and analysis reports.

Below is an Entity Relationship Diagram (ERD) of the TMDb database:

<img src="https://github.com/Explore-AI/Pictures/blob/master/TMDB_ER_diagram.png?raw=true" width=70%/>

As can be seen from the ERD, the TMDb database consists of `12 tables` containing information about movies, cast, genre, and so much more.

# 🚀 Approach

1. **Database Setup**

    - The `TMDB` dataset was provided in SQLite format (`TMDB.db`), making it serverless and easy to integrate with Jupyter.
    
    - The `%load_ext` sql command was used to activate SQL queries in Jupyter.
  
    - The `%sql sqlite:///TMDB.db` establish a connection to the local database using the '%sql' magic command.

2. **Exploratory Queries**

    - **Investigated movie metadata:** oldest movies, most popular genres, and companies with the highest average popularity.
    
    - Explored **actor/actress details**: roles played by **Vin Diesel**, movies featuring **Alan Rickman**, and award nominations for actors.
    
    - Analyzed **Oscar awards data**: identifying winners, normalizing inconsistent year formats, and counting unique award categories.
  
3. **Analytical Tasks**

    - Found movies between certain release dates with budget and popularity constraints.
    
    - Calculated intersections of genres and keywords (e.g., Thriller movies containing “love”).
    
    - Examined female actors with names starting with “**N**”.
    
    - Checked which award categories had the highest number of actor nominations.
  
4. **Data Integrity & Cleaning**

    - Addressed formatting inconsistencies (e.g., Oscars year field pre-1934).
    
    - Ensured normalization concepts were understood (avoiding redundancy, ensuring uniqueness, reducing anomalies).
  
5. **Presentation & Portfolio**

    - Queries were modularized into `.sql` files for reuse.
    
    - Results were exported as `.csv` and presented in tables within the **README** using Markdown.
    
    - Explanations and insights were documented alongside queries for storytelling in data analysis.

## 📑 Project Table of Contents

| #  | Question                                                                 | Query and Solution |
|----|--------------------------------------------------------------------------|---------------------|
| 1  | Who won the Oscar for “Actor in a Leading Role” in 2015?                 | [Query_1.ipynb](notebooks/Query_1.ipynb) |
| 2  | What query will produce the ten oldest movies in the database?           | [Query_2.ipynb](notebooks/Query_2.ipynb) |
| 3  | How many unique awards are there in the Oscars table?                    | [Query_3.ipynb](notebooks/Query_3.ipynb) |
| 4  | How many movies are there that contain the word “Spider” within their title? | [Query_4.ipynb](notebooks/Query_4.ipynb) |
| 5  | How many movies are there that are both in the "Thriller" genre and contain the word “love” anywhere in the keywords? | [Query_5.ipynb](notebooks/Query_5.ipynb) |
| 6  | How many movies are there that were released between 1 August 2006 ('2006-08-01') and 1 October 2009 ('2009-10-01') that have a popularity score of more than 40 and a budget of less than 50 000 000?                 | [Query_6.ipynb](notebooks/Query_6.ipynb) |
| 7  | How many unique characters has "Vin Diesel" played so far in the database?           | [Query_7.ipynb](notebooks/Query_7.ipynb) |
| 8  | What are the genres of the movie “The Royal Tenenbaums”?                    | [Query_8.ipynb](notebooks/Query_8.ipynb) |
| 9  | What are the three production companies that have the highest movie popularity score on average, as recorded within the database? | [Query_9.ipynb](notebooks/Query_9.ipynb) |
| 10  | How many female actors (i.e. gender = 1) have a name that starts with the letter "N"?                | [Query_10.ipynb](notebooks/Query_10.ipynb) |
| 11  | Which genre has, on average, the lowest movie popularity score?           | [Query_11.ipynb](notebooks/Query_11.ipynb) |
| 12  | Which award category has the highest number of actor nominations (actors can be male or female)? (Hint: Oscars.name contains both actors' names and film names.)                    | [Query_12.ipynb](notebooks/Query_12.ipynb) |
| 13  | DStv will be having a special week dedicated to the actor Alan Rickman. Write a query that would create a new view that shows the titles, release dates, taglines, and overviews of all movies that Alan Rickman has played in? | [Query_13.ipynb](notebooks/Query_13.ipynb) |




