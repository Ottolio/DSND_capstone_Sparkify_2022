# DSND_capstone_Sparkify_2022
Capstone project for Udacity data scientist course

## Installation
The code was run on the Udacity workspace. Running the code should also be possible with the Anaconda distribution of Python 3.6 on a computer with pyspark 2.4 and java installed.
 
### Data
mini_sparkify_event_data ... 128 MB, provided by Udacity.
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
This is the final project of Udacity's Data Scientist course. I chose the Spark project over the other options in order to learn more from the course. Extracurricular lessons were also provided on Spark by Udacity.

## Procedure

The data was exploratorily analyzed before defining the features with which to model the property "churning" (quitting) or "not-churning" the imaginary Sparkify service.

Features that were used:
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

The following algorithms were used
   1) Logistic Regression
   2) Random Forest
   3) Gradient-Boosted Trees
   4) Naive Bayes

As mentioned in the project description, F1-score evaluation was used due to the skewed data.

### Performance of the modelling, results on the Train- and Test-set and duration of computation

|F1_train|F1_test|minutes|algorithm|
|-----|----|-------|---------|
|0.694 | 0.791 | 3.7 min | 1) Logistic Regression     |
|0.834 | **0.845** | 1.1 min | 2) **Random Forest**          |
|0.769 | 0.774 | 8.3 min | 3) Gradient-Boosted Trees |
|0.644 | 0.744 | 0.1 min | 4) Naive Bayes            |

The best prediction of the test data, i.e. "which user has churned" was usually achieved with the Random Forest classification algorithm.

The train data was usually fitted with an F1-Score close to and smaller to the test data, suggesting there is little to no overfitting.

The whole notebook usually took about half an hour to compile.


## Licensing, Authors, Acknowledgements

Must give credit to Udacity for the Sparkify Event data.

In order to overcome challenges on the local laptop and the workspace provided by Udacity, several resources have been used. Besides the extracurricular course on Spark from Udacity, the websites [stockoverflow](https://stackoverflow.com/), github and pyspark documentation have been used.
