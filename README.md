# IMDB-Python-Project-
Objective 
Objective of this project is to explore the  IMPDB movies dataset and find the insights Regading 
Best and Worst Movie by certain paramters sich as reveneue , profit , budget , ROI , No of votes , popularity ,rating  (we can do that seperately and by creating the function as well )
Are Francise More Sucessfull ?
Most Sucessfull Directors by multiple parametres and drill down the finidng generes as well .
Scuessfull Actors Analysis 
Analysing Movie Genres 

We have poster links as well so we can handle that by 
from IPython.display import HTML
subset = df[[Columns list ]].head()
HTML(subset.to_html(escape=False))

Data Overview 
id: The ID of the movie (clear/unique identifier).
title: The Official Title of the movie.
tagline: The tagline of the movie.
release_date: Theatrical Release Date of the movie.
genres: Genres associated with the movie.
belongs_to_collection: Gives information on the movie series/franchise the particular film belongs to.
original_language: The language in which the movie was originally shot in.
budget_musd: The budget of the movie in million dollars.
revenue_musd: The total revenue of the movie in million dollars.
production_companies: Production companies involved with the making of the movie.
production_countries: Countries where the movie was shot/produced in.
vote_count: The number of votes by users, as counted by TMDB.
vote_average: The average rating of the movie.
popularity: The Popularity Score assigned by TMDB.
runtime: The runtime of the movie in minutes.
overview: A brief blurb of the movie.
spoken_languages: Spoken languages in the film.
poster_path: The URL of the poster image.
cast: (Main) Actors appearing in the movie.
cast_size: number of Actors appearing in the movie.
director: Director of the movie.
crew_size: Size of the film crew (incl. director, excl. actors).
