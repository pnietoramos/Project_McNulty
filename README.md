# Can you recommend me a book?
### Domain
We aim to analyze books by different features and classify them in three classes: "Life changing", "Ok" and "Rather watch TV".
A database with information of more than 30000 books is available in www.kaggle.com.
The ratings for new and other books not included in the list can be classified using this algorithm and used by readers as a guide for good reading.

### Data
Our classification will be based in the rating_average parameter.

| Variable                        | Description                               |
|---------                        |--------                                |  
| author                          | Book author                           |   
| original_publication            | Publication year                      |
| language_code                   | Language                              |
| work_text_reviews               | Number of written reviews (?)
| ratings_1                       | Number of reviews from source 1          |
| ratings_2                       | Number of reviews from source 2          |
| ratings_3                       | Number of reviews from source 3          |
| ratings_4                       | Number of reviews from source 4          |

### Known unknowns
 The boundaries based in ratings_1 for the three classes will be decided on the basis of making the "Life changing" class small (~5%).

 The correlation between number of ratings for the different sources has to be evaluated. If they are very correlated they will be eliminated. In that case the number of variable could be too small and new features will be needed.

 The authors can be arbitrarily associated with a number to be included in the analysis.
