# Time Series Forecasting for Bitcoin

## Overview
This notebook presents an exploration of time series forecasting applied to Bitcoin prices. It encompasses a variety of forecasting models ranging from simple baselines to advanced neural network architectures. The aim is to predict future Bitcoin prices by analyzing historical data, employing different strategies to evaluate their performance and applicability in real-world scenarios.

## Notebook Main Sections:
- **Quick EDA (Exploratory Data Analysis)**: Initial data loading and exploration to understand the trends and patterns in Bitcoin prices.
- **Evaluation Functions**: Implementation of functions to evaluate model performance.
- **Modeling Experiments**: Multiple forecasting models are explored, including naive forecasts, dense models, Conv1D, LSTM, and a replication of the N-Beats algorithm.
- **Multivariate Time Series Forecasting**: Expanding the forecasting models to consider multiple variables.
- **Ensemble and Advanced Modeling**: Exploring ensemble techniques and building models to predict future prices outside of the training dataset `forecasting the future`.
- **Confidence Interval Estimation**: Applying the bootstrap method to get prediction intervals, enhancing decision-making under uncertainty.
- **Visualizations**: Detailed plots and visualizations to illustrate model performances and predictions.

## Modeling Expriments results
| Model                | MAE         | MSE           | RMSE         | MAPE       | MASE       |
|----------------------|-------------|---------------|--------------|------------|------------|
| naive_model          | 495.359161  | 5.859700e+05  | 765.486755   | 1.813522   | 1.005668   |
| model_1_dense_w7_h1  | 496.785339  | 5.857107e+05  | 765.317383   | 1.826456   | 1.008563   |
| model_2_dense_w30_h1 | 517.390320  | 6.108959e+05  | 781.598328   | 1.914533   | 1.056179   |
| model_3_dense_w30_h7 | 1090.221802 | 2.829687e+06  | 1257.680054  | 4.045431   | 2.219269   |
| model_4_CONV1D       | 503.955292  | 5.992592e+05  | 774.118347   | 1.856972   | 1.023119   |
| model_5_LSTM         | 508.647949  | 6.115502e+05  | 782.016785   | 1.873066   | 1.032646   |
| model_6_multivariate | 497.548553  | 5.888026e+05  | 767.334717   | 1.828983   | 1.010113   |
| model_8_NBEATs       | 501.481262  | 5.984253e+05  | 773.579529   | 1.844809   | 1.018097   |
| model_9_ensemble     | 497.354370  | 5.868772e+05  | 766.079102   | 1.829250   | 1.009718   |
| model_10_turkey      | 8948.126953 | 1.330372e+08  | 10994.261719 | 41.444145  | 15.708638  |


<img src="images\visualization.png" />

## Forecasted Bitcoin prices visualization

<img src="images\forecasting predictions.png" />

