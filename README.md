# Project Info
- **Georgetown University Data Science and Analytics**
- **Course**: Massive Data Fundamentals 502 Project
- **Contributors**: Kuiyu Zhu, Guiming Xu, Zihao Zhou, Yuxuan Yao
- **Contact**:(kz175, gx26, zz267, yy560)@georgetown.edu

# Dataset
- [Global Surface Summary of Day](https://registry.opendata.aws/noaa-gsod/)
- **Amazon Resource Name (ARN)**: `arn:aws:s3:::aws-gsod`
- **Size**: 20.1 GB
- **Description**: GSOD is a collection of daily weather measurements (temperature, wind speed, humidity, pressure, and more) from 9000+ weather stations around the world.
- **License**: The data is intended for free and unrestricted use in research, education, and other non-commercial activities. Per World Meteorological Organization (WMO) Resolution 40, redistribution of these data by others must provide this same notification, and non-U.S. data cannot be redistributed for commercial purposes.

# Introduction
In many cases, the weather forecast plays a very important role in life. If people predict that it will rain tomorrow, they will prepare the umbrella in advance. If they know the temperature of tomorrow, they will prepare the appropriate apparel. We can make various predictions based on the daily data of global surface.

* [`Tornado_RF.ipynb`](https://github.com/gu-yuxuanyao/502Project/blob/master/Tornado_RF.ipynb): This program selects 13 columns as features and _Tonado_ as the label. This program contains many statistics plots to help us to understand the features and their importance, which are implemented by `Correlation` and `seaborn`. The main classification is used in this program is `RandomForestClassifier` and the evaluation method is `BinaryClassificationEvaluator`. 

* [`temp_predicton.ipynb`](https://github.com/gu-yuxuanyao/502Project/blob/master/temp_predicton.ipynb): This program selects 10 columns as features and _Mean_Temp_ as the label. This program implements `LinearRegression` to do the model processing and __LASSO Regression__ is used by adjusting the parameters _egParam_ and _elasticNetParam_ to select the better predictors. The evaluation method is `RegressionEvaluator`.

* [`rain_prediction(LR&DT).ipynb`](https://github.com/gu-yuxuanyao/502Project/blob/master/rain_prediction(LR%26DT).ipynb): This program selects 14 columns as the predictors and _Rain_or_Drizzle_ as the label we need to predict. This program mainly implements the `LogisticRegression`, `DecisionTreeClassifier` and `RandomForestClassifier` to do the classification models and the evaluation method is `BinaryClassificationEvaluator`. 

* All programs apply pipeline for the machine learning processing. [`REPORT_ANLY-502 Weather Prediction Project Report.pdf`](https://github.com/gu-yuxuanyao/502Project/blob/master/REPORT_ANLY-502%20Weather%20Prediction%20Project%20Report.pdf) contains all the details about our project.

# Thank you and have a nice day! :)
