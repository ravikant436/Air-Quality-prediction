# Air Quality Prediction - Bangalore City
<a href="https://github.com/ravikant436/Air-Quality-prediction/commits/master" target="_blank">
  <img src="https://img.shields.io/github/last-commit/ravikant436/Air-Quality-prediction?style=flat-square" alt="GitHub last commit">
</a>

<a href="https://github.com/ravikant436/Air-Quality-prediction/issues" target="_blank">
  <img src="https://img.shields.io/github/issues/ravikant436/Air-Quality-prediction?style=flat-square&color=red" alt="GitHub issues">
</a>

<a href="https://github.com/ravikant436/Air-Quality-prediction/pulls" target="_blank">
  <img src="https://img.shields.io/github/issues-pr/ravikant436/Air-Quality-prediction?style=flat-square&color=blue" alt="GitHub pull requests">
</a>

<a href="https://github.com/ravikant436/Air-Quality-prediction#contribute" target="_blank">
  <img alt="Contributors" src="https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square">
</a>

<a href="https://standardjs.com" target="_blank">
  <img alt="ESLint" src="https://img.shields.io/badge/code_style-standard-brightgreen.svg?style=flat-square">
</a>
<hr>

Air quality is measured with the Air Quality Index(PM 2.5). 
PM 2.5 is a fine particulate matter that is an air pollutant that is a concern for people’s health when levels in the air are high.

In this Project, We aim to predict PM 2.5 of Bangalore City for a given values of different parameters like Temprature, Visibility, Wind speed etc.

# Table of contents

- [Usage](#usage)
- [Data Description](#Data-Description)
- [Feature Importance](#Features-Importance)
- [Model Evaluation](#Model-Evaluation)
- [Deployment](#Deployment)

# Usage

Project is ready to run (with some requirements). You need to clone and run:
```sh
pip install -r requirements.txt
```

After installing all required libraries. Open command prompt, navigate to project folder and run:
```sh
python app.py
```

# Data Description

### Data Collection
Data was scrapped from Web (https://en.tutiempo.net/climate/ws-432950.html) for years 2013-2018

**Requests** and **BeautifulSoup** modules were used for web scrapping. Complete code is present in <a href="https://github.com/ravikant436/Air-Quality-prediction/blob/main/AQI_Data_collection.ipynb">AQI_Data_collection.ipynb</a> 

### Dataset Columns Description

<table>
  <tr><td>T</td><td>Average Temperature (°C)</td></tr>
  <tr><td>TM</td><td>Maximum temperature (°C)</td></tr>
  <tr><td>Tm</td><td>Minimum temperature (°C)</td></tr>
  <tr><td>SLP</td><td>Atmospheric pressure at sea level (hPa)</td></tr>
  <tr><td>H</td><td>Average relative humidity (%)</td></tr>
  <tr><td>VV</td><td>Average visibility (Km)</td></tr>
  <tr><td>V</td><td>Average wind speed (Km/h)</td></tr>
  <tr><td>VM</td><td>Maximum sustained wind speed (Km/h)</td></tr>
  <tr><td>PM 2.5</td><td>Air Quality Index</td></tr>
</table>

# Features Importance

### Features Importance Graph

<img src="https://github.com/ravikant436/Air-Quality-prediction/blob/main/images/feature-importance.png"/>

### Co-relation Heatmap between all the features

<img src="https://github.com/ravikant436/Air-Quality-prediction/blob/main/images/corr-graph-aqi.png"/>

# Model Evaluation

We have considered all 8 features in Model Building. Various Regressor Models have been tried out. 

Find the code and score of all the Models under Regression Section in <a href="https://github.com/ravikant436/Air-Quality-prediction/blob/main/Air_quality_prediction.ipynb">Air_quality_prediction.ipynb</a>

### Linear Regression
**RMSE Score:** 60.7

<img src="https://github.com/ravikant436/Air-Quality-prediction/blob/main/images/linear_regression.png" />

### Lasso 
**RMSE Score:** 60.2

<img src="https://github.com/ravikant436/Air-Quality-prediction/blob/main/images/lasso.png" />

### Random Forest Regressor
**Hypertuned Parameters**: {'n_estimators': 500, 'min_samples_split': 2, 'min_samples_leaf': 1, 'max_features': 'sqrt', 'max_depth': 15}

**RMSE Score:** 41.3

<img src="https://github.com/ravikant436/Air-Quality-prediction/blob/main/images/random_forest.png" />

### KNN Regressor
**RMSE Score:** 54.5

**Hyperturned K**: 3

<img src="https://github.com/ravikant436/Air-Quality-prediction/blob/main/images/knn-tuning.png" />

Distplot:

<img src="https://github.com/ravikant436/Air-Quality-prediction/blob/main/images/knn.png" />

# Deployment

Among above tested Models, Random Forest Regressor has shown best performance in comparison, on our dataset. 

So we have created pickel file of the same, <a href="https://github.com/ravikant436/Air-Quality-prediction/blob/main/random_forest_model.pkl">random_forest_model.pkl</a>

We are using Flask Framework, and project will be deployed on Heroku (**Work in Progress**)
