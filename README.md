# Can you recommend me a book? (Not doable with the data set)
### Domain
The database can be found in [www.kaggle.com](https://www.kaggle.com/zygmunt/goodbooks-10k).

### Data

| Variable                        | Description                           |
|---------                        |--------                               |  
| author                          | Book author                           |   
| original_publication            | Publication year                      |
| language_code                   | Language                              |
| work_text_reviews               | Number of written reviews (?)         |
| ratings_1                       | Number of ratings with 1 star         |
| ratings_2                       | Number of ratings with 2 stars        |
| ratings_3                       | Number of ratings with 3 stars        |
| ratings_4                       | Number of ratings with 4 stars        |

### Known unknowns
The features rating_i are the number of ratings with i stars.
There are not enough features.


If possible I would like to change the topic of the project to:

# Detecting failures in Scania trucks
### Domain
We want to deal here with the diagnostics of malfunctioning trucks of the Scania brand.
The aim of the project will be to be able to identify or discard one of the possible causes for the vehicule failure.
Although we have no knowledge on the truck mechanics and possible causes of the different types of failures this does not pose a problem on the view of the available data that will be described.  

### Data
Data set for this project can be found in [www.kaggle.com](https://www.kaggle.com/uciml/aps-failure-at-scania-trucks-data-set).
Sensor readings for 76000 Scania trucks with some kind of failure are listed.
The description of the readings are not given due to proprietary reasons but two different type of features are given.
A column labeled "class" identify those trucks with a failure in the Air Pressure Systems from those with other type.
Two types of features are available: 100 single numerical counters (100 columns) and 7 histogram variables for which counts for 10 bins are given (70 columns).
For the histogram variables the lowest and highest bis are open and, hence, cover a broader range than the other bins.

| Variable                                  | Description                  |
|---------                                  |--------                      |  
|aa-af; ah-ax; bb-cm; co-cr; ct-ed, ef, eg  |single numerical counters     |
|ag, ay, az, ba, cn, cs, ee                 |histogram variables           |                                         

### Known unknowns  

The large number of features in this problem is quite high and could be problematic for getting a good accuracy.

Specifically, descriptive information about the features is not given and therefore none of them can be discarded on this basis.

About 5% of the entries contain at least NaN values.
These data can not be simply discarded beacause that will reduce the application of the model.  
A solution would be to substitute the value for a (-1) times mean for that feature.
This will numerically account for the malfunction of that reading which could be valuable information.
