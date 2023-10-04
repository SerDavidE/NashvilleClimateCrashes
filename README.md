
![copy_banner_5](https://github.com/SerDavidE/NashvilleClimateCrashes/assets/138124275/b455389e-172d-4fcb-b457-1edcdcd90882)

## Analyzing Climate's Role in Accidents in Nashville, U.S.A.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset Overview](#dataset-overview)
3. [Data Exploration, Cleaning, and Transformation](#data-exploration)
4. [Exploratory Data Analysis (EDA)](#eda)
5. [Statistical Tests](#statistical-tests)
6. [Model Building and Evaluation](#model-building)
7. [Insights, Conclusions, and Recommendations](#insights)
8. [Future Work](#future-work)

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
The features curated for this purpose included weather variables and lagged values of "Total Accidents".

### Model Training
Each model was subjected to rigorous training, inclusive of hyperparameter tuning and optimization.

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

## <a name="future-work"></a>8. Future Work
### Improvements
Subsequent iterations might witness refined model optimizations and the inclusion of granular data to enhance insights.
