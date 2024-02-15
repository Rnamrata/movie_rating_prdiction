# movie_rating_prediction

This project is based on the movie recommendation system. There are four different datasets. The training dataset with columns userId, movieId, rating, and timestamp The given movie dataset of ratings given by users for a particular movie on a 0-5 star scale. The test dataset with columns userId, movieId, and timestamp.The movies dataset with columns movieId, title, and genres. The links dataset with columns movieId, imdbId, and tmdbId.The main purpose of this project is to build a user-based collaborative system and predict movie ratings. Apart from that a content-based movie recommendation system and a recommendation for new users have been done in this project.

Here is the brief of the code:

At first, after loading and checking the data info of all four datasets the movies dataset has been merged with the training and testing dataset based on the movie IDs. Then the training dataset was analyzed through a few processes to understand the data in a better way.

In the data pre-processing step, one-hot encoding was used to extract the features.

In collaborative filtering, cosine similarity was used to measure the similarity between user vectors in the user-item interaction matrix. The resulting similarity matrix was used to identify similar movies for recommendation purposes. In user-based collaborative filtering, the user vectors represent users based on their ratings for movies, and cosine similarity can be calculated to find users with similar preferences. A movie rating prediction was made using the Singular Value Decomposition (SVD) from the surprise library. 3-fold cross-validation was on the training dataset to calculate Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Mean Absolute Error (MAE). Then the prediction was done on the test dataset. Moreover, the train_test_split() method was used to estimate the Mean Squared Error (MSE), Root Mean Squared Error (RMSE) of the Mean Squared Error (MSE), Root Mean Squared Error (RMSE).

Final Score:

Mean Squared Error (MSE): 77.60%
Root Mean Squared Error (RMSE): 88.09%.


 
