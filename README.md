# **IMDB Python Project** ![Icon](https://img.icons8.com/ios-filled/50/000000/movie.png)

## **Objective**

The goal of this project is to explore the IMDB movies dataset and gain insights into various aspects of movies, including:

- **Best and Worst Movies**: Analyze movies based on parameters such as revenue, profit, budget, ROI, number of votes, popularity, and rating. We will explore these metrics both separately and using custom functions.
- **Franchise Success**: Determine if movie franchises are more successful compared to standalone movies.
- **Successful Directors**: Identify the most successful directors based on multiple parameters and drill down into findings by genre.
- **Successful Actors**: Analyze the success of actors in the dataset.
- **Movie Genres**: Analyze and evaluate movie genres.

## **Data Overview**

The dataset contains the following columns:

- **id**: The unique identifier for the movie.
- **title**: The official title of the movie.
- **tagline**: The tagline of the movie.
- **release_date**: The theatrical release date of the movie.
- **genres**: Genres associated with the movie.
- **belongs_to_collection**: Information on the movie series or franchise the film belongs to.
- **original_language**: The language in which the movie was originally shot.
- **budget_musd**: The budget of the movie in million dollars.
- **revenue_musd**: The total revenue of the movie in million dollars.
- **production_companies**: Production companies involved in making the movie.
- **production_countries**: Countries where the movie was shot or produced.
- **vote_count**: The number of votes by users on TMDB.
- **vote_average**: The average rating of the movie.
- **popularity**: The popularity score assigned by TMDB.
- **runtime**: The runtime of the movie in minutes.
- **overview**: A brief summary of the movie.
- **spoken_languages**: Languages spoken in the film.
- **poster_path**: The URL of the poster image.
- **cast**: Main actors appearing in the movie.
- **cast_size**: Number of actors appearing in the movie.
- **director**: Director of the movie.
- **crew_size**: Size of the film crew (excluding actors).

## **Handling Poster Links**

To display movie posters alongside other movie details, use the following code snippet:

```python
from IPython.display import HTML

# Select the relevant columns and display the first few rows with poster links
subset = df[['title', 'poster_path', 'overview']].head()
HTML(subset.to_html(escape=False))
