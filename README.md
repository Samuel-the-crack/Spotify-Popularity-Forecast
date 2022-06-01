# Spotify-Popularity-Forecast
Basic implementation of machine learning using K-Nearest-Neighbor (KNN)

![github-small](https://github.com/Samuel-the-crack/Spotify-Popularity-Forecast/blob/main/Spotify%20Header.png)

## Spotify Popularity forecast using KNN
Spotify is the biggest music streaming platform, in this repo I want to make a model where the target is 'Popularity' based on 'acousticness', 'danceability', 'energy', 'instrumentalness', 'liveness', 'loudness', 'speechiness', 'tempo', 'valence', and 'popularity'. This model using [K-Nearest-Neighbor (KNN)](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html). The input of this model is a dataset and the desired output is model's accuracy in form of lineplot.

Requirement : numpy, pandas, matplotlib, seaborn, and sci-kit learn (sklearn)

## Overview 
I'm using 'Spotify_Data.csv' as the main data, you can check more about this dataset [here](https://www.kaggle.com/code/vatsalmavani/music-recommendation-system-using-spotify-dataset/data). After importing the dataset I'm limitting the year (2010 - 2020), after that I'm take the featured column. The next step is I'm defining the x (independent variable) and y variables to split the data into training and test using `from sklearn.model_selection import train_test_split`. The last thing is applying KNN model using `from sklearn.neighbors import KNeighborsClassifier`, and it's accuracy using `from sklearn.metrics import accuracy_score` and then plotting it using seaborn lineplot. 

![github-small](https://github.com/Samuel-the-crack/Spotify-Popularity-Forecast/blob/main/lineplot_Acc.png)

As we can see the lineplot above the accuracy is quite low, it's because the independent variable not highly affect the target which is 'Popularity'.
