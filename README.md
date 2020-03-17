#  Distributed Computing Project: Air Quality Index Prediction with Spark ML and H2O

## Contributors:
- Wenjie Duan
- Xuxu Pan
- Peng Liu
- Jingxian Li
- Min Che

## Data:
- Daily AQI Dataset in United States from 1980-2019
- Weather information: Wind, Temperature, Barometric Pressure, RH and Dewpoint

## Project Goal:
- Investigate How Weather Influence AQI
- Investigate How Historical AQI correlated with future AQI

## Implementation:
- Data sotraged in AWS S3
- Processed time series data, and joined AQI table and Weather table
- Implemented SparkRandomForest, H2ODeepLearningEstimator with different cluster setting
- Analysed feature importance for AQI prediction 

## Conclusion:
- Time series model is important for air quality forecast
- H2O deep learning models performs better than Random Forest models 
- Models trained on larger dataset performs better than those trained on smaller dataset
- Execution time decrease when cluster specs change from xlarge to 2xlarge, however, more nodes do not guarantee higher time efficiency 
