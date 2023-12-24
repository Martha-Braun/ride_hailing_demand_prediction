# ride_hailing_demand_prediction

## Context 
For my Master Thesis I investigated the performance of different time series models for demand prediction of ride-hailing services (e.g. Uber, Lyft). I used the dataset published by the NYC Taxi & Limousine Commission (find it [here](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page))

## Methodology
Three models have been tested, with growing complexity: the statistical model SARIMA, the machine learning model Prophet, and the deep learning model Temporal Fusions Transformer (TFT). Prophet has been developed by Facebook in 2017 and TFT by Google in 2021. Both algorithms have been successful in their respective fields of applications, namely social media interaction predictions and e-commerce predictions. The aim is to analyze the performance of these algorithms for ride-hailing demand prediction. 

## Conclusion
The models are being compared based on their RMSE and MASE error value. The results show that SARIMA has the highest error value, mainly because it was unable to detect all patterns occurring in the time series. TFT performs best in terms of error values. However, with a training time of 30 min it is not very efficient to implement in a business product. Additionally, TFT requires a lot of manual hyperparameter tuning to reach the lowest error value. Prophet’s performance is very close to the TFT performance, with a training time of less than one minute. It is also a very user-friendly library that requires no manual tuning and offers various features to do time series analysis.
