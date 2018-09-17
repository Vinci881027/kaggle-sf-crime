# Kaggle San Francisco Crime Classification

An end to end project to explore, visualize, and analyze San Francisco crime data and predict category of crime given temporal and spatial features.

## Installation
All Python packages required for this project are located in the [requirements.txt](https://github.com/k-chuang/kaggle-sf-crime/blob/master/requirements.txt) and can be installed via the command below.

`pip install -r requirements.txt`

## Files

**Data Exploration & Visualization**
- [kaggle-sf-crime-exploration.ipynb](https://github.com/k-chuang/kaggle-sf-crime/blob/master/kaggle-sf-crime-exploration.ipynb) - jupyter notebook with initial data explorations & visualizations of SF crime

**Data Mining & Machine Learning**
- [kaggle-sf-crime-project.ipynb](https://github.com/k-chuang/kaggle-sf-crime/blob/master/kaggle-sf-crime-project.ipynb) - jupyter notebook with end to end data science workflow, such as data preprocessing, feature engineering, building baseline models, model selection, hyperparameter tuning, and Kaggle submission.

**Hyperparameter Tuning Results**
- [cv_results](https://github.com/k-chuang/kaggle-sf-crime/blob/master/cv_results) - folder containing the hyperparameter tuning results (CV scores (mean & standard deviation) and hyperparameters) at each iteration of Bayesian Optimization.

## Dataset
Dataset contains incidents derived from SFPD Crime Incident Reporting system. The data ranges from **1/1/2003 to 5/13/2015** (~12 years worth of data). The training set and test set rotate every week, meaning week 1,3,5,7,... belong to test set, week 2,4,6,8,... belong to training set.

#### Data Fields
- **Dates** - timestamp of the crime incident
- **Category** - category of the crime incident (only in train.csv). This is the target variable you are going to predict.
- **Descript** - detailed description of the crime incident (only in train.csv)
- **DayOfWeek** - the day of the week
- **PdDistrict** - name of the Police Department District
- **Resolution** - how the crime incident was resolved (only in train.csv)
- **Address** - the approximate street address of the crime incident
- **X** - Longitude
- **Y** - Latitude

The source of the dataset can be found in the following links:
- [Kaggle Source](https://www.kaggle.com/c/sf-crime/data)
- [Original Source](https://data.sfgov.org/Public-Safety/-Change-Notice-Police-Department-Incidents/tmnf-yvry/about)

## License

See the [LICENSE](https://github.com/k-chuang/kaggle-sf-crime/blob/master/LICENSE) file for license rights and limitations (MIT).
