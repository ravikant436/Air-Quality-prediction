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

Air quality is measure with the Air Quality Index(PM 2.5)

PM 2.5 is a fine particulate matter that is an air pollutant that is a concern for people’s health when levels in the air are high.

# Table of contents

- [Usage](#usage)
- [Data Description](#Data-Description)
- [Feature Importance](#Feature-Importance)
- [Model Building](#model-building)
- [Deployment](#deployment)
- [Conclusion](#conclusion)

# Usage

Project is ready to run (with some requirements). You need to clone and run:
```sh
pip install -r requirements.txt
```

After installing all required libraries. Open command prompt, navigate to project folder and run:
```sh
python app.py
```

# Data-Description

### Data Collection
Data was scrapped manually from Web (https://en.tutiempo.net/climate/ws-432950.html) for years 2013-2018
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

# Features-Importance

### Features Importance Graph

<img src="https://github.com/ravikant436/Air-Quality-prediction/blob/main/images/feature-importance.png"/>

### Co-relation Heatmap between all the features

<img src="https://github.com/ravikant436/Air-Quality-prediction/blob/main/images/corr-graph-aqi.png"/>

# Contributor
<table>
  <tr>
    <td align="center"><a href="https://github.com/ravikant436"><img src="https://github.com/ravikant436/ravikant436.github.io/blob/main/images/photo-1.jpeg" width="100px;" alt=""/><br /><sub><b>Ravikant Tyagi</b></sub></a><br /></td>
  </tr>
</table>
