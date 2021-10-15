# Will It Rain Tomorrow?
Predicting rain is a thing, as all human activities will be influenced by rain. Especially in agricultural sector, 
forecasting the rainfall will help the farmers and other related parties.

## Context
This aim of this project is to predict the next-day rain with some information relating to the weather. 
The target variable is binary. And through this project, binary classification will be carried out 
with various classifaction methods to find the best model that suits the case. 
Data exploration also will be done to identify the characteristics of the data.

## Dataset
The dataset was taken from [Kaggle](https://www.kaggle.com/jsphyg/weather-dataset-rattle-package).
This dataset contains about 10 years of daily weather obeseravtions per day from many location throughout Australia.\
Here are some information about the variables that used in the dataset:
### Target Variable
RainTomorrow: This means, Did it rain the nex day? **Yes** or **No**
### Input Variables
- Date: The date of observation
- Location: The common name of the location of the weather station
- MinTemp: The minimum temperature in degrees celcius
- MaxTemp: The maximum temperature in degrees celcius
- Rainfall: The amount of rainfall recorded for the day in mm
- Evaporation: The so-called Class A pan evaporation (mm) in the 24 hours to 9am
- Sunshine: The number of hours of bright sunshine in the day
- WindGustDir: The direction of the strongest wind gust in the 24 hours to midnight
- WindGustSpeed: The speed (km/h) of the strongest wind gust in the 24 hours to midnight
- WindDir9am: Direction of the wind at 9am
- WindDir3pm: Direction of the wind at 3pm
- WindSpeed9am: Wind speed (km/hr) averaged over 10 minutes prior to 9am
- WindSpeed3pm: Wind speed (km/hr) averaged over 10 minutes prior to 3pm
- Humidity9am: Humidity (percent) at 9am
- Humidity3pm: Humidity (percent) at 3pm
- Pressure9am: Atmospheric pressure (hpa) reduced to mean sea level at 9am
- Pressure3pm: Atmospheric pressure (hpa) reduced to mean sea level at 3pm
- Cloud9am: Fraction of sky obscured by cloud at 9am. This is measured in "oktas", which are a unit of eigths. It records how many eigths of the sky are obscured by cloud. A 0 measure indicates completely clear sky whilst an 8 indicates that it is completely overcast.
- Cloud3pm: Fraction of sky obscured by cloud (in "oktas": eighths) at 3pm. See Cload9am for a description of the values
- Temp9am: Temperature (degrees C) at 9am
- Temp3pm: Temperature (degrees C) at 3pm
- RainToday: Boolean: 1 if precipitation (mm) in the 24 hours to 9am exceeds 1mm, otherwise 0

## Python Library Used
- numpy
- pandas
- patplotlib
- seaborn
- from scipy import stats
- from sklearn.preprocessing import MinMaxScaler
- from sklearn.model_selection import train_test_split
- from sklearn.linear_model import LogisticRegression
- from sklearn-neighbors import KNeighborsClassifier
- from sklearn.tree import DecisionTreeClassifier
- from sklearn.ensemble import RandomForestClassifier
- from sklearn.metrics import accuracy_score, confusion_matrix, classification_report

## Exploratory Data Analysis
- Dataset shape
- Dataset info
- Dataset descripcion (Descriptive Statistics)
- Data visualisation (Boxplot, Histogram, Barplot, Pie Chart, Scatter Plot, Heatmap)
- Correlation

## Pre-processing Process
- Checking missing value
- Dropping unnecessary columns
- Missing value imputation
- Outliers Detection using Z-score
- Handling outliers
- One-Hot Encoding
- Scaling Data

## Model Building
- Logistic Regression
- K-Nearest Neighbors
- Decision Tree/ CART
- Random Forest

## Model Evaluation
- Accuracy
- Confusion Matrix
- Classification Report (Precision, Recall, F1-Score)

## Source & Acknowledgements
Observations were drawn from numerous weather stations. The daily observations are available from http://www.bom.gov.au/climate/data \
An example of latest weather observations in Canberra: http://www.bom.gov.au/climate/dwo/IDCJDW2801.latest.shtml \
\
Definitions adapted from http://www.bom.gov.au/climate/dwo/IDCJDW0000.shtml \
Data source: http://www.bom.gov.au/climate/dwo/ and http://www.bom.gov.au/climate/data \
\
Copyright Commonwealth of Australia 2010, Bureau of Meteorology.
