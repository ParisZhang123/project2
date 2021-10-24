# Project 2
This project is aiming to provide advise for property investors who are looking to purchase property in NSW.
We extract data from Domain.com and collecting supportive data from official websites such as ABS and data.gov.au to provide analysis of current market trend and predict future trending of NSW real estate.
The main machine learning utilized including Linear Regression and Random Forest. 
In this project, we are using different features to predict Sydney House Price trending in relation to both Microeconomic and Macroeconomic factors.
![5 Warilla Place](https://user-images.githubusercontent.com/86837854/138535868-cbc8a55e-51be-4c30-9113-ae3a828e436e.jpg)
 
---
Random Forest Model
---
We are predicting Sydney House Price trending in Macroeconomic perspective by utilizing Random Forest Model. Features we think would related to Sydney house pricing include CPI (Consumer Price Index), Interest rate (RBA cash rate), GDP (Gross Domestic Product), and AUD/USD exchange rate. 
In this model, we import RandomForestClassifier and RandomeForestRegressor from sklearn.ensemble, StandardScaler from sklearn.preprocessing, train_test_split from sklear.model_selection, confusion_metrix, accuracy_score and classification_report from sklearn.metrics. We also import Dense from tensorflow.jeras.layers, Sequential from tensorflow.keras.models to proceed the analysis. In this model, we firstly cleaning feature data which were extracted from data.gov.au and ABS, then concat dataframes into one for feature variables followed by cross-referencing data extract from Domain API which is used as target variable. After that, we build and fit those variables into Random Forest Regressor Model.  We also plotted those features to provide more visualized data. Finally, we train a neural network model to predict Sydney house price to see whether it may rise or fall in the future.
![CPI_png](https://user-images.githubusercontent.com/86837854/138587062-482f5934-199f-438f-bf0c-323b8bba713d.PNG)
![cashrate_png](https://user-images.githubusercontent.com/86837854/138587070-6a1a55fd-7708-4cb7-9827-d37177e9a669.PNG)
![audusd_price_png](https://user-images.githubusercontent.com/86837854/138587074-809e89ba-3a7f-494a-b7f0-14cabce9bef3.PNG)

The data in this model is on annual basis which is from year 2011 to year 2021.

Linear Regression Model
---
We are also predicting Sydney House Price based on Microeconomic factors. We believe features such as income level, education level, distance from major employment centre, local crime rate, number and ranking of schools in LGA are main factors effecting house price. 
