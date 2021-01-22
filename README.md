# spotifygenreclassifier
Given a playlist URI, the genres of the songs in it are predicted.

# Summary
Using the Spotify API, get your client ID and client secret. Go to https://developer.spotify.com/documentation/web-api/ to do that.
A training dataframe has to be built so multiple spotify playlists with predefined genres are considered, and to the created dataframe, an extra column called 'genre' is added.
All the dataframes made are combined into a single one, and standardized. X and y are created and split into testing and training data. Different prediction models are applied
and the best one is chonsen based on the accuracy. In this instance, Random Forest was the best one. To make the predictions better, hyperparameter tuning was attempted. It didn't make much of a difference. Bagging or boosting can make a better impact, which will be added in the future. With the best version of Random Forest, predictions are made for a given playlist.
