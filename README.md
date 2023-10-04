
![copy_banner_5](https://github.com/SerDavidE/NashvilleClimateCrashes/assets/138124275/b455389e-172d-4fcb-b457-1edcdcd90882)

> **Note**: This README provides a summarized overview of the project. For a comprehensive analysis, detailed methodology, and in-depth discussions, please refer to the [accompanying research paper](link_to_pdf_in_your_repository).

## Analyzing Climate's Role in Accidents in Nashville, U.S.A.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset Overview](#dataset-overview)
3. [Data Exploration, Cleaning, and Transformation](#data-exploration)
4. [Exploratory Data Analysis (EDA)](#eda)
5. [Statistical Tests](#statistical-tests)
6. [Model Building and Evaluation](#model-building)
7. [Insights, Conclusions, and Recommendations](#insights)
8. [Limitations](#limitations)
9. [Future Work](#future-work)
10. [Acknowledgments](#acknowledgments)

## <a name="introduction"></a>1. Introduction
### Objective
The project's primary objective is to discern the impact of diverse weather conditions on traffic accidents' frequency in selected U.S. cities, emphasizing Nashville.

### Overview
This endeavor encompasses a meticulous journey through data exploration, cleaning, transformation, exploratory data analysis, statistical testing, model building, and evaluation. The goal is to unveil patterns, seasonal tendencies, and insights detailing the relationship between diverse weather variables and accident frequency.

## <a name="dataset-overview"></a>2. Dataset Overview
### Description
The dataset proffers a detailed perspective on weather conditions, geographical specifics, and accident timestamps across Nashville, Madison, and Boise. It encapsulates features such as Season, Temperature(C), Visibility(km), Weather_Condition, Precipitation(mm), and Total Accidents.

### Source
The datasets are sourced from Kaggle:

- [Global Daily Climate Data](https://www.kaggle.com/datasets/guillemservera/global-daily-climate-data) - Licensed under Attribution-NonCommercial 4.0 International (CC BY-NC 4.0).
  
- [US Accidents](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents) - Licensed under Attribution-NonCommercial 4.0 International (CC BY-NC 4.0).

## <a name="data-exploration"></a>3. Data Exploration, Cleaning, and Transformation
### Initial Exploration
The outset witnessed a detailed examination of the dataset's structure, the identification of missing values, and a brief dive into the fundamental statistical properties inherent in the variables.

### Data Cleaning
This phase was earmarked by addressing missing values, outliers, and undertaking essential data type conversions to ensure the sanctity and consistency of data.

### Transformation
The transformations employed revolved around adept feature engineering, which involved spawning lagged values of the pivotal target variable and scaling the data to meet model prerequisites.

## <a name="eda"></a>4. Exploratory Data Analysis (EDA)
### Univariate Analysis
This step involved dissecting individual variable distributions using tools like histograms and boxplots, revealing profound insights into variable distributions and the presence of extreme values.

### Bivariate Analysis
The analysis focused on the intricate relationships between weather variables and accident incidence, utilizing scatter plots and correlation matrices, and subsequently unveiling significant correlations between the variables.

### Time-Series Analysis
This entailed the decomposition of accident data to shed light on trends, seasonality, and intrinsic patterns.

## <a name="statistical-tests"></a>5. Statistical Tests
### Tests Performed
Tests were orchestrated to emphasize correlations and seasonality, authenticating the significance of observed patterns and relationships.

### Results
The results cemented the presence of significant correlations and seasonal trends in the dataset, accentuating the role of weather variables as potential precursors in model building.

## <a name="model-building"></a>6. Model Building and Evaluation
### Model Selection
A spectrum of models, encompassing SARIMA, Random Forest, XGBoost, LightGBM, and LSTM, were chosen due to their versatility in handling multifaceted input features.

### Feature Selection
For the machine learning models, the features selected included:
- Lagged values of the target variable "Total Accidents", considering a weekly seasonality of 7 days.
- A subset of weather variables that potentially impact accident rates, such as `Temperature(C)`, `Visibility(km)`, and `Wind_Speed(kmh)`.

### Model Training
- **Data Splitting:** For this project, 80% of the data was utilized for training and the remaining 20% for testing.
  
- **SARIMA:** Leveraging the stationarity and identified seasonality of the series, a Seasonal ARIMA (SARIMA) model was employed. SARIMA models cater to seasonality in time series data.
  
- **Machine Learning Models:** Post SARIMA, machine learning models like Random Forest and Gradient Boosting Machines (XGBoost & LightGBM) were explored, using pertinent features and lagged values as predictors.
  
- **LSTM Model:** An exploration into Long Short-Term Memory (LSTM) models was also conducted. LSTMs, a subtype of recurrent neural networks (RNNs), are adept at capturing long-term dependencies, making them apt for time series forecasting tasks.

### Model Evaluation
Evaluation metrics like MAE, RMSE, and MAPE were employed to appraise the models on their testing set performance.

### Model Comparison
A comprehensive juxtaposition was conducted, shedding light on each model's aptitude and predictive capabilities.

## <a name="insights"></a>7. Insights, Conclusions, and Recommendations
### Insights
The analysis delineated the profound impact of weather conditions on traffic accidents, emphasizing the significance of these meteorological facets.

### Conclusions
The expedition through the dataset culminated in the realization that weather conditions, notably in Nashville, are pivotal determinants in traffic accidents' incidence. Gradient boosting models like LightGBM showcased superior performance, emphasizing the judicious selection of models based on the dataset's inherent characteristics.

### Recommendations
Recommendations span across proactive weather-based traffic management, predictive interventions, raising public awareness, and infrastructural enhancements to ensure safety.

## <a name="limitations"></a>8. Limitations
The analysis conducted has several limitations, including:
- **Tourism Impact**: Seasonal tourism influxes, which can increase traffic, were not considered.
- **Road Maintenance**: Ongoing constructions and the general road conditions, which can affect accident rates, were not included.
- **Traffic Congestion**: Factors such as traffic density and rush hour patterns were not explored.
- **Driving Behavior**: Local driving habits and issues like driving under influence were not investigated.
- **Vehicle Types**: The variety of vehicles on the roads was not analyzed.
- **Public Transportation**: The efficiency and utilization of public transportation, which can influence the number of vehicles on the road, were not considered.

## <a name="future-work"></a>9. Future Work
### Improvements:
- **Model Enhancement:** Refine models using advanced techniques like Bayesian optimization.
- **Feature Augmentation:** Explore rolling averages and advanced lag features.
- **Data Expansion:** Integrate hourly weather conditions and real-time traffic data for richer insights.
- **Broadened Analysis:** Extend the study to more cities for generalized conclusions.

### Extensions:
- **Additional Factors:** Consider variables like wind speed, humidity, and road conditions.
- **Advanced Models:** Experiment with deep learning models, such as Transformers, for forecasting.
- **Real-Time System:** Develop a system for dynamic risk assessment using live weather data, supporting proactive traffic management.

## <a name="acknowledgments"></a>10. Acknowledgments
Gratitude is extended to the individuals and organizations that have generously provided the datasets and to the open-source communities that have been instrumental in the project's fruition. Additionally, my gratitude to my mentors and peers at WBS Coding School for their continuous support and valuable feedback.
