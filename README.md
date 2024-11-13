# Airbnb and Bitcoin Data Analysis and Forecasting

## Project Overview

This project is a comprehensive analysis of two popular time series datasets: **Airbnb listings** and **Bitcoin prices**. The goal is to preprocess the data, perform exploratory data analysis (EDA), apply clustering and anomaly detection, and forecast future trends using automated machine learning (AutoML).

## Table of Contents

- [Project Overview](#project-overview)
- [Datasets](#datasets)
- [Project Workflow](#project-workflow)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Clustering and Anomaly Detection](#clustering-and-anomaly-detection)
- [Modeling and Forecasting](#modeling-and-forecasting)
- [Technologies Used](#technologies-used)
- [Results](#results)
- [Contributors](#contributors)

---

## Datasets

Added datasets in respective folders.

1. **Airbnb New York City Data**:
   - **Source**: [New York City Airbnb Open Data](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)
   - **Description**: A dataset of Airbnb listings in New York City with features like neighborhood, room type, price, and availability.

2. **Bitcoin Historical Data**:
   - **Source**: [Bitcoin Historical Data](https://www.kaggle.com/datasets/sudalairajkumar/cryptocurrencypricehistory)
   - **Description**: Historical daily prices of Bitcoin including opening, closing, high, and low prices, along with trading volume.

## Project Workflow

1. **Data Preprocessing**: Clean and prepare the data for analysis.
2. **EDA**: Visualize and analyze trends, seasonal patterns, and anomalies.
3. **Clustering and Anomaly Detection**: Apply K-Means for clustering and Isolation Forest for anomaly detection.
4. **Modeling and Forecasting**: Build forecasting models using AutoML tools to predict future trends.

## Data Preprocessing

### Airbnb Data
- **Missing Values**: Filled using forward-fill and backward-fill methods.
- **Encoding**: Categorical features such as `neighborhood` and `room type` are label-encoded.
- **Scaling**: Numerical features (e.g., `price`, `availability_365`) are scaled for clustering.

### Bitcoin Data
- **Date Conversion**: Converted the date column to datetime format and set as the index.
- **Missing Values**: Missing values filled via forward-fill.
- **Scaling**: Standardized key features (e.g., `Close`, `Volume`) for clustering.

## Exploratory Data Analysis (EDA)

1. **Airbnb Data**: 
   - Distribution of prices by neighborhood and room type.
   - Time series analysis of listing availability and prices.
   - Volume of listings in each neighborhood.

2. **Bitcoin Data**:
   - Trend analysis of Bitcoin closing prices over time.
   - Seasonal decomposition of Bitcoin prices.
   - Distribution of trading volume and price changes.

## Clustering and Anomaly Detection

### K-Means Clustering
- **Airbnb Data**: Clustered listings based on price, availability, and room type.
- **Bitcoin Data**: Clustered on closing price and trading volume to identify patterns.

### Anomaly Detection with Isolation Forest
- **Airbnb Data**: Detected outliers in listing prices and availability.
- **Bitcoin Data**: Identified anomalous price spikes or drops.

## Modeling and Forecasting

### Airbnb Forecasting
- **Target Variable**: `price`
- **Method**: Used PyCaret's AutoML to build regression models for forecasting prices based on neighborhood, room type, and historical data.
<img width="779" alt="image" src="https://github.com/user-attachments/assets/b17a11f6-d42b-49d5-b65a-2083fe92b000">


### Bitcoin Forecasting
- **Target Variable**: `Close` price
- **Method**: Built time series models using PyCaret for forecasting future prices and identifying market trends.
<img width="1013" alt="image" src="https://github.com/user-attachments/assets/efd7ae3e-bf4f-4f97-b4ae-03853735598a">


## Technologies Used

- **Python**: Core language for data manipulation and analysis.
- **Pandas**: Data manipulation.
- **Matplotlib & Seaborn**: Visualization.
- **Scikit-Learn**: Clustering and anomaly detection.
- **PyCaret**: Automated machine learning and forecasting.
- **AutoVIML**: Ensemble modeling for Airbnb and Bitcoin forecasting.

## Results

- **Airbnb Analysis**: Identified key price patterns across neighborhoods and room types, detected price anomalies, and forecasted future listing prices.
- **Bitcoin Analysis**: Visualized Bitcoin’s price trends, identified anomalies, and forecasted future price movements.

## Contributors

- **Apurva Karne**
- **Contact**: apurva.karne@sjsu.edu

---
