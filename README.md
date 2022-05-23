# DSND_capstone_Sparkify_2022
Capstone project for Udacity data scientist course

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
This is the final project of Udacity's D96064a2ta Scientist course. I chose to Spark project over the other options in order to learn even more from the course. Extracuricular lessons were also provided on Spark.

## Procedure

The data was exloratorily analysed before defining the features with which to model the property "churning" (quitting) or "not-churning" the imaginary Sparkify service.

LFeatures that were used:
```
features:
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

### Supervised-learning classification algorithms

The followign algorithms were used
   1) Logistic Regression
   2) Random Forest
   3) Gradient-Boosted Trees
   4) Naive Bayes

As mentioned in the project description, F1-score evaluation was be used due to the skewed data.

### Performance of the modelling, results on the Train- and Test-set and duration of computation

   F1 Scores
   
| train  ||  test  || minutes

0.751 | 0.652 | 3.9 min .... 1) Logistic Regression

0.851 | 0.802 | 1.0 min .... 2) Random Forest

0.784 | 0.751 | 7.9 min .... 3) Gradient-Boosted Trees

0.694 | 0.638 | 0.1 min .... 4) Naive Bayes

The best prediction of the test data, i.e. "which user has churned" was achieved with the Random Forest classification algorithm.

The train data was also fitted with an F1-Score close to and smaller to the test data, suggesting there is little to no overfitting.

The whole notebook took aber half an hour to compile.


## Licensing, Authors, Acknowledgements

Must give credit to Udacity for the Sparkify Event data.

In order to overcome challenges on the local laptop and the workspace provided by Udacity, several resources have been used. Besides the extracuricular course on Spark from Udacity, the websites [stockoverflow](https://stackoverflow.com/), github and pyspark documentation have been used.
