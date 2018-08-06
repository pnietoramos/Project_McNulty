# The Forest Buddy
### Domain
The project aim is two fold. Firstly we want to build a model for the prediction for the identification of high risk for wildfires. Secondly the prediction for the the cover vegetation that will be regenerated in the point in the unfortunate event of a fire effectively taking place is foreseen. The models will be based on cartographic data alone discarding any need for on site data collection.

### Data
Data set for this project can be found in [www.kaggle.com](https://www.kaggle.com/uciml/forest-cover-type-dataset).
Cartographic data for more than half a million points from the Roosevelt National Forest of northern Colorado are available. The available features are:

| Features (**Labels to classify**)   | Range [units]       | Description                           |
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
| Wilderness_AreaX (4 binary columns) | 0-1                 | Wilderness area X within the forest         |
| Soil_TypeX (40 binary columns)      | 0-1                 | Soil type X of the area        |
|**Cover_Type**                        | 0-7                | Label for type of cover        |
|**Horizontal_Distance_To_Fire_Points**| 0-7173 [meters]    | Horizontal distance to the nearest ignition points       |

### Known unknowns  

The Wilderness_AreaX features are only relevant for the particular data collected at the Roosevelt National Forest and will be discarded.  
The Soil_TypeX features are redundant and will be substituted by a single feature with range (1-40) labeling the soil type.  
The large amount of data could make the most computationally intensive methods too expensive to be used in the modeling.    
