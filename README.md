# Movie Recomendation System

A Deepnote project that uses movie based data to do Popularity-Based Filtering, Content-Based Filtering and Collaborative-Based Filtering.

Notebook 1: Popularity-Based Filtering 

 In this notebook, we develop a model to recommend popular movies to the user. The process begins by loading data files from IMDB and implementing a weighted rating formula. Subsequently, we filter the movies, ensuring they have a vote count greater than or equal to 'm,' where 'm' is the minimum vote count threshold. Next, we apply the weighted rating function to the movies and add the resulting weighted ratings to the dataframe. Finally, we use these ratings to filter for the top 'x' number of movies.
 
Notebook 2: Content-Based Filtering

 In this notebook, we developed content-based filtering. This was achieved by using the movie data, particularly the 'overview' field, to generate a similarity matrix. To ensure the flexibility of querying any movie in the dataset, we created a function called 'similar_movies' that takes 'movie_title' and 'nr_movies' as parameters. This function allows you to specify a movie and retrieve the top 'x' similar movies to display.
 
Notebook 3: Collaborative-Based Filtering

  The objective of this task was to predict user preferences for movies based on their ratings. We began by processing the reviews data and converting it into a scikit-learn dataset. Next, we constructed the training dataset, which is utilized to train the SVD model from the Surprise library. Once the model is trained, we can make predictions by providing the user ID and movie ID. Finally, we validate the model to assess its accuracy and ensure that its predictions align well with actual user ratings. We use both the Root Mean Square Error (RMSE) and Mean Absolute Error (MAE) as evaluation metrics.
