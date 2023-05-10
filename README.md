# Real-Estate-Valuation-Prediction

## **Dataset**:
•	Dataset was taken from Kaggle.

•	The dataset https://www.kaggle.com/datasets/dskagglemt/real-estate-valuation-by-uci

•	Attribute Information: The inputs are as follows

X1=the transaction date (for example, 2013.250=2013 March, 2013.500=2013 June, etc.)

X2=the house age (unit: year).

X3=the distance to the nearest MRT station (unit: meter)

X4=the number of convenience stores in the living circle on foot (integer)

X5=the geographic coordinate, latitude. (unit: degree)

X6=the geographic coordinate, longitude. (unit: degree)

The output is as follow
Y= house price of unit area

# Exploratory Data Analysis :
## Heatmap of variables :
![Corr](https://github.com/Prajyotc/Real-Estate-Valuation-Prediction/assets/115527993/f3ad243f-5295-46dc-8d1d-e7bf1ee05412)

## Scatter plots :
![Scatter](https://github.com/Prajyotc/Real-Estate-Valuation-Prediction/assets/115527993/8ef1f28f-9868-47d3-bce3-26c316fc8a13)

## Histogram :
![Hist](https://github.com/Prajyotc/Real-Estate-Valuation-Prediction/assets/115527993/98eb7faa-0975-42ba-a5c4-77c5ddc0dcd0)

•	Log transformed histogram of distance_to_the_nearest_MRT_station
![hist trans](https://github.com/Prajyotc/Real-Estate-Valuation-Prediction/assets/115527993/1cb9151e-77e8-4b5e-8e7d-2d6720f5b2ad)

## Model Fitting :

Fitted the Ordinary Least Square Regression model.
## Model summary
1)	R² is computed without centering  since the model does not contain a constant.
2)	 Standard Errors assume that the covariance matrix of the errors is correctly specified.
From the summary output of regression model, it can be concluded that model is statistically significant. The R squared for the model is 0.89 i.e., around 89% of total variation in the response house price can be explained by the predictor variables.
 From summary output, it can be drawn that house age is not significantly contributing in the prediction of house price.
Model can be given as,
House price = -0.3037(House age) +27.5531(Distance from the nearest metro station) + 48.690*(number of convenient stores)

## Conclusion:
Starting with loading the data so far, we have done EDA, null values treatment, feature selection and then model building. The R squared of our model is **89%** which can be said to be good for this dataset. This performance could be due to various reasons like: no proper pattern of data, not enough relevant features.

