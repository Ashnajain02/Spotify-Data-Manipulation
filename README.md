# Spotify-Data-Manipulation

Part 1: Unsupervised Learning 


My data was a list of tracks, and the features of the tracks such as energy, danceability, temp etc. The clusters that were created were clusters of songs that most resembled each other in regards to the features. In short, the songs that were most like each other. 


An example of  a cluster made was of slow songs (All of Me by John Legend, and Let Her Go by Passenger) compared to another cluster that included upbeat songs (Wake Me Up by Avicii, and Cheerleader by OMI)


Part 2: Supervised Learning


The goal was to predict the target y variable (danceability) by using the following x variables (energy, key, loudness, mode, speechiness, acousticness, instrumentals, liveness, valence, tempo, duration_ms, time_signature, and track_name). 


I implemented 2 different models: Decision Trees and K-Nearest Neighbors.


For Decision Trees, the parameters used to tune to increase performance were criterion, splitter, and max_depth.
* criterion: the function to measure the quality of a split
* splitter: the strategy used to choose the split at each node
* max_depth: the maximum depth of the tree


For K-Nearest Neighbors, the parameters used to tune to increase performance were n_neighbors, algorithm, and metric.
* N_neighbors: the number of neighbors to use by default for k-neighbors queries
* Algorithm: the algorithm used to compute the nearest neighbors
* Metric: is the distance metric to use for the tree


The purpose of using the tunable parameters is to receive a higher accuracy tune model when compared to the base model. Since this is a regression problem, I used RMSE (Root Mean Square Error) to evaluate the performance of the model.


When looking at the RMSE scores, the RMSE score dropped from 0.21 to 0.14 for Decision Trees and stayed at 0.15 for both models for K-Nearest Neighbor. To see a significant change in RMSE scores, it would be beneficial to have a larger dataset.
