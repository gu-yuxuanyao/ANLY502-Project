# Project Info
- **Course**: Data Science and Analytics 502 Project
- **Contributors**: Kuiyu Zhu, Guiming Xu, Zihao Zhou, Yuxuan Yao
- **E-mail**:(kz175, gx26, zz267, yy560)@georgetown.edu

# Dataset
- [Global Surface Summary of Day](https://registry.opendata.aws/noaa-gsod/)
- **Amazon Resource Name (ARN)**: `arn:aws:s3:::aws-gsod`
- **Size**: 20.1 GB
- **Description**: GSOD is a collection of daily weather measurements (temperature, wind speed, humidity, pressure, and more) from 9000+ weather stations around the world.
- **License**: The data is intended for free and unrestricted use in research, education, and other non-commercial activities. Per World Meteorological Organization (WMO) Resolution 40, redistribution of these data by others must provide this same notification, and non-U.S. data cannot be redistributed for commercial purposes.

# Introduction
In many cases, the weather forecast plays a very important role in life. If people predict that it will rain tomorrow, they will prepare the umbrella in advance. If they know the temperature of tomorrow, they will prepare the appropriate apparel. We can make various predictions based on the daily data of global surface.
* [`rain_prediction(LR&DT).ipynb`](https://github.com/gu-yuxuanyao/502Project/blob/master/rain_prediction(LR%26DT).ipynb): This program selects 14 columns as the predictors and _Rain_or_Drizzle_ as the label we need to predict. This program mainly implements the `LogisticRegression` and `DecisionTreeClassifier` to do the classification models and the evaluation method is `BinaryClassificationEvaluator`. 
* [`temp_predicton.ipynb`](https://github.com/gu-yuxuanyao/502Project/blob/master/temp_predicton.ipynb): This program selects 10 columns as features and _Mean_Temp_ as the label. This program implements `LinearRegression` to do the model processing and __LASSO Regression__ is used by adjusting the parameters _egParam_ and _elasticNetParam_ to select the better predictors. The evaluation method is `RegressionEvaluator`.
* Both programs apply pipeline for the machine learning processing.
