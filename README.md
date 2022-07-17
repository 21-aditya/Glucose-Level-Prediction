# Project by
1. Aditya Ramachandran
2. Shreya Ananth
3. Chiran Jeevi MP

From College of Engineering, Guindy, Anna University

# Glucose-Level-Prediction
Type-1 diabetes is a very common disorder which currently affects a variety of the world’s population, majority being 0-16years of age. It’s an auto-immune disorder in which the beta cells of the pancreas does not produce insulin and have to be given externally with the help of insulin shots.

This project aims in predicting blood glucose levels that help in optimising closed-loop insulin delivery systems. The glucose level prediction is done first as a univariate time-series prediction using Auto Regressive Integrated Moving Average (ARIMA) model and Recurrent Neural Network (RNN) which takes as input, only the CGM data. Their performances are compared.

Then, for more accurate predictions, several external factors like type of meal, insulin dosage and time of meal are also taken to predict glucose level as a multivariate time-series using Convolutional Neural Network(CNN) and Recurrent Neural Network(RNN). Depending on the above mentioned features, an estimate of the blood glucose levels of the person at 15 and 60 minute intervals can be predicted.

We have also tried to classify foods as low-GI or high-GI based on subsequent cgm trends after meal intake

# RESULTS
1. Univariate Time Series Prediction using ARIMA Model
<table>
  <tr>
    <td>
<img src="https://github.com/21-aditya/Glucose-Level-Prediction/blob/Computer_Science/Results/UnivariateTimeSeriesPrediction-ARIMA2.png" width="100%" height="100%" align="left">
    </td>
  </tr>
</table>
2. Univariate Time Series Prediction using LSTM Model
<table>
  <tr>
    <td>Actual</td>
    <td>Predicted</td>
  </tr>
  <tr>
    <td>
<img src="https://github.com/21-aditya/Glucose-Level-Prediction/blob/Computer_Science/Results/UnivariateLSTM-Actual.png" width="100%" height="100%" align="left">
    </td>
    <td>
<img src="https://github.com/21-aditya/Glucose-Level-Prediction/blob/Computer_Science/Results/UnivariateLSTM-Predicted.png" width="100%" height="100%" align="left">
    </td>
  </tr>
</table>
3. Multivariate Time Series Prediction using CRNN Model
<table>
  <tr>
    <td>Actual</td>
    <td>Predicted</td>
  </tr>
  <tr>
    <td>
<img src="https://github.com/21-aditya/Glucose-Level-Prediction/blob/Computer_Science/Results/MultiVariate-Actual.png" width="100%" height="100%" align="left">
    </td>
    <td>
<img src="https://github.com/21-aditya/Glucose-Level-Prediction/blob/Computer_Science/Results/MultiVariate-Predicted.png" width="100%" height="100%" align="left">
    </td>
  </tr>
</table>
4. Clustering food as high-GI and low-GI
<table>
  <tr>
    <td>Low GI</td>
    <td>High GI</td>
  </tr>
  <tr>
    <td>
<img src="https://github.com/21-aditya/Glucose-Level-Prediction/blob/Computer_Science/Results/Cluster1-LowGI.png" width="100%" height="100%" align="left">
    </td>
    <td>
<img src="https://github.com/21-aditya/Glucose-Level-Prediction/blob/Computer_Science/Results/Cluster2-HighGI.png" width="100%" height="100%" align="left">
    </td>
  </tr>
</table>

# REFERENCES
[1]	T. Hamdi et al., “Artificial neural network for blood glucose level prediction,” in 2017 International Conference on Smart, Monitored and Controlled Cities (SM2C), 2017.

[2]	K. Li, J. Daniels, C. Liu, P. Herrero, and P. Georgiou, “Convolutional recurrent neural networks for glucose prediction,” IEEE J. Biomed. Health Inform., vol. 24, no. 2, pp. 603–613, 2020.

[3]	S. Mirshekarian, R. Bunescu, C. Marling, and F. Schwartz, “Using LSTMs to learn physiological models of blood glucose behavior,” Annu Int Conf IEEE Eng Med Biol Soc, vol. 2017, pp. 2887–2891, 2017.

[4]	W. P. T. M. van Doorn et al., “Machine learning-based glucose prediction with use of continuous glucose and physical activity monitoring data: The Maastricht Study,” PLoS One, vol. 16, no. 6, p. e0253125, 2021.

[5]	S. Mirshekarian, H. Shen, R. Bunescu, and C. Marling, “LSTMs and neural attention models for blood glucose prediction: Comparative experiments on real and synthetic data,” Annu Int Conf IEEE Eng Med Biol Soc, vol. 2019, pp. 706–712, 2019.
