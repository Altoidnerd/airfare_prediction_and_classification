# Airfare prediction and classification

A machine learning exercise presenting a simple model for 

*	(1) prediction of airfares from the data contained in the search query using linear support vector regression implementation sklearn.SVM.LinearSVR.
*	(2) classification of flight itinerary search results by likelihood the returned fare will ultimately be purchased by the consumer, using simple Naive Bayes implementation in sklearn. 



## Getting Started
The discussion is contained in the two ipython notebooks 
* 	```fare_regression.ipynb```
*	```booking_classifier.ipynb```.  

These files contain code that will mostly work out of the box, but that depends on the existence of three csv files containing datasets in the working directory:
 
*	```airport_data.csv``` 
*	```booking_data.csv```
*	```search_data.csv```

Due to github filesize restrictions, ```search_data.csv``` was partitioned and zipped.  To recover the original ```search_data.csv``` file, simply run the following to generate search_data.csv


```
me@myshell $ unzip search_data_1.zip && unzip search_data_2.zip && cat search_data_1.csv search_data_2.csv > search_data.csv && du -h
```

The output should look like 

```
search_data.csv
Archive:  search_data_1.zip
  inflating: search_data_1.csv
Archive:  search_data_2.zip
  inflating: search_data_2.csv
581M	search_data.csv
```

You should be ready to go.

```
me@myshell $ jupyter notebook fare_regression.ipynb &
me@myshell $ jupyter notebook booking_classifier.ipynb &
```
