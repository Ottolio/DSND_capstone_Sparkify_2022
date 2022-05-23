# DSND_capstone_Sparkify_2022
Capstone pfoject for Udacity data scientist course

## Installation
The code was run on the Udacity workspace. Running the code shoudl also be possible with the Anaconda distribution of Python 3.6 on a computer with pyspark 2.4 and java installed.
 
### Data
mini_sparkify_event_data ... 128MB, provided by Udacity.
```
Columns:
 |-- artist
 |-- auth
 |-- firstName
 |-- gender
 |-- itemInSession
 |-- lastName
 |-- length
 |-- level
 |-- location
 |-- method
 |-- page
 |-- registration
 |-- sessionId
 |-- song
 |-- status
 |-- ts
 |-- userAgent
 |-- userId
```

## Aim of project
This is the final project of Udacity's DAta Scientist course. I chose to Spark project over the other options in order to learn even more from the course. Extracuricular lessons were also provided on Spark.

## Results
List of used features
```
data
 |--userID
 |--gender
 |--churn
 |--level
 |--platform
 |--state
 |--numEvents
 |--regDays
 |--ratioAddFriend
 |--ratioAddtoPlaylist
 |--ratioNextSong
 |--ratioRollAdvert
 |--ratioThumbsDown
 |--ratioThumbsUp
 |--ratioFirstHalf
 |--ratioArtists
 |--numPerSession
 |--timePerEvent
```

### Supervised-learning classification algorithms used

1) Logistic Regression
2) Random Forest
3) Gradient-Boosted Trees
4) Naive Bayes

As mentioned mentioned in the project description F1-score evaluation was be used.

### Results on the Train- and Test-set and duration of computation




## Licensing, Authors, Acknowledgements

Must give credit to Udacity for the Sparkify Event data.

In order to overcome challenges on the local laptop and the workspace provided by Udacity, several resources have been used. Besides the extracuricular course on Spark from Udacity the webistes [stockoverflow](https://stackoverflow.com/) and pyspark documentation have been used extensively. 
Also code from github has been used, namely from the following programmers: mx404, angang-li, chziha, u1up0ng, danieljaensch and russom.

Spark MLlib: Main Guide

Otherwise, feel free to use the code here as you would like! 
