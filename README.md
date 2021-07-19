# spotifygenreclassifier
Given a playlist URI, the genres of the songs in it are predicted.

## Summary:
Using the Spotify API, get your client ID and client secret. Go to https://developer.spotify.com/documentation/web-api/ to do that.
A training dataframe has to be built so multiple spotify playlists with predefined genres are considered, and to the created dataframe, an extra column called 'genre' is added.
All the dataframes made are combined into a single one, and standardized. X and y are created and split into testing and training data. Different prediction models are applied
and the best one is chonsen based on the accuracy. In this instance, Random Forest was the best one. To make the predictions better, hyperparameter tuning was attempted. 
It didn't make much of a difference. Bagging or boosting can make a better impact, which will be added in the future. With the best version of Random Forest, predictions are made
for a given playlist.

## Playlist in this instance:
https://open.spotify.com/user/kazu8l2llhpll0uobr3wmdt5f/playlist/3aFp6OcR1rukcTX0A8ppxe?si=whfMK89nR6ytz0xRcq8jVQ
![image](https://user-images.githubusercontent.com/57229722/106105386-ef594f00-6169-11eb-971d-7fa728234d5b.png)

## Results:
![image](https://user-images.githubusercontent.com/57229722/126142504-d50eda18-a6ab-4b55-9368-e7e6443d7fb0.png)

## Takeaway:
Songs don't commit to a single genre so with the basic method that this project does, the accuracy won't be great. There is some area of improvement however, perhaps by using bagging/boosting as mentioned earlier, or by bringing in the tensorflow library. 
Hopefully something I will work on in the future.
