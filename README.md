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

   
