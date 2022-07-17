# Glucose-Level-Prediction
Type-1 diabetes is a very common disorder which currently affects a variety of the world’s population, majority being 0-16years of age. It’s an auto-immune disorder in which the beta cells of the pancreas does not produce insulin and have to be given externally with the help of insulin shots.

This project aims in predicting blood glucose levels that help in optimising closed-loop insulin delivery systems. The glucose level prediction is done first as a univariate time-series prediction using Auto Regressive Integrated Moving Average (ARIMA) model and Recurrent Neural Network (RNN) which takes as input, only the CGM data. Their performances are compared.

Then, for more accurate predictions, several external factors like type of meal, insulin dosage and time of meal are also taken to predict glucose level as a multivariate time-series using Convolutional Neural Network(CNN) and Recurrent Neural Network(RNN). Depending on the above mentioned features, an estimate of the blood glucose levels of the person at 15 and 60 minute intervals can be predicted.

We have also tried to classify foods as low-GI or high-GI based on subsequent cgm trends after meal intake
