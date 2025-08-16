# 🎬 Movie Database Analysis (Serverless SQL with Jupyter Notebook)

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

| Query ID | Question | SQL File | Result |
|----------|----------|----------|--------|
| Q1       | Thriller movies with "love" in keywords | [query1.sql](queries/query1.sql) | [Result](results/query1_result.csv) |
| Q2       | Movies released 2006–2009 with budget < 50M & popularity > 40 | [query2.sql](queries/query2.sql) | [Result](results/query2_result.csv) |
| Q3       | Top 3 production companies by avg popularity | [query3.sql](queries/query3.sql) | [Result](results/query3_result.csv) |





