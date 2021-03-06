# Predicting the prices of Fiat 500 with Linear Regression

## Introduction

The purpose of this model is to apply the Linear Regression in order to predict the prices of three differen classes of Fiat 500. The dataset comes from [Kaggle.](https://www.kaggle.com/)
For additional information about Linear Models you can read my article on [Towards Data Science.](https://towardsdatascience.com/machine-learning-observe-how-a-linear-model-works-by-predicting-the-prices-of-the-fiat-500-fb38e0d22681?source=friends_link&sk=1efb890e3ca5747c8aee0b57500c710e)

## Description of the dataset

- model: pop, lounge, sport

- engine_power: Kw of the engine

- age_in_days: age of the car in days 

- km: kilometres of the car

- previous_owners: number of previous owners

- lat: latitude of the seller (the price of cars in Italy varies from North to South of the country)

- lon: longitude of the seller (the price of cars in Italy varies from North to South of the country)

- price: selling price

## Usage
```python
import sklearn 
from sklearn.model_selection import train_test_split
from sklearn import preprocessing
from sklearn.linear_model import LinearRegression
from scipy import stats
import seaborn as sns
import matplotlib.pyplot as plt
from matplotlib.pyplot import figure
import numpy as np
import scipy as sp
import pandas as pd
```
## Exploratory Data Analysis

Scatter matrix for model, engine_power, age_in_days, km and price
![alt text](img/scatter_matrix.JPG)

Correlation matrix for model, age_in_days, km and price
![alt text](img/heatmap.JPG)

## Model performance - comparison between the actual values and the predicted values
![alt text](img/histogram_residuals.JPG)

## Score

- Training set score: 0.83
- Test set score: 0.85

## License
The dataset for this model comes from [Kaggle.](https://www.kaggle.com/)
