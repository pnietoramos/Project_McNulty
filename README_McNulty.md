# The Forest Buddy
### Domain



### Data
Data set for this project can be found in [www.kaggle.com](https://www.kaggle.com/uciml/forest-cover-type-dataset).
Cartographic data for more than half a million points from the Roosevelt National Forest of northern Colorado are available. The available features are:


| Features                           | Range [units]        | Description                           |
|---------                            |--------             |--------                               |  
| Elevation                           | 1859-3858 [meters]  | Elevation above sea level in meters   |   
| Aspect                              | 0-360 [degrees]     | Orientation of the slope relative to North direction  |
| Slope                               | 0-66 [degrees]      | Slope at the point                  |
| Horizontal_Distance_To_Hydrology    | 0-1397 [meters]     | Horizontal distance to nearest water surface     |
| Vertical_Distance_To_Hydrology      | -173-601[meters]    | Vertical distance to the nearest water surface         |
| Horizontal_Distance_To_Roadways     | 0-7117 [meters]     | Horizontal distance to the nearest roadway        |
| Hillshade_9am                       | 0-254               | Hillshade index (gray scale) at 9am, summer solstice        |
| Hillshade_Noon                      | 0-254               | Hillshade index (gray scale) at Noon, summer solstice         |
| Hillshade_3pm                       | 0-254               | Hillshade index (gray scale) at 3pm, summer solstice         |
| Wilderness_AreaX (4 binary columns) | 0-1                 | Wilderness area within the forest         |
| Soil_TypeX (40 binary columns)      | 0-1                 | Soil type of the area        |
| *Horizontal_Distance_To_Fire_Points*| 0-7173 [meters]     |        |
| *Cover_Type*                          | 0-7                 |         |


### Known unknowns  

The large number of features in this problem is quite high and could be problematic for getting a good accuracy.

Specifically, descriptive information about the features is not given and therefore none of them can be discarded on this basis.

About 5% of the entries contain at least NaN values.
These data can not be simply discarded beacause that will reduce the application of the model.  
A solution would be to substitute the value for a (-1) times mean for that feature.
This will numerically account for the malfunction of that reading which could be valuable information.
