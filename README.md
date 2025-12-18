# Stock_Market_Prediction
This is our application for our Final Project Submission (DSCI 6007-02) Distributed and Scalabale Data Engineering.
The app.py contains the flask code and html files all should be stored in templates folder.

The link to our presentation video : https://youtu.be/52LJ4wKdnpM

## Overview

This repository contains a **Stock Market Prediction** application developed as the final project for **DSCI 6007-02: Distributed and Scalable Data Engineering (Spring 2023)**. The project focuses on analyzing historical stock market data and predicting future stock prices using **Long Short-Term Memory (LSTM)** neural networks. In addition to the machine learning pipeline, the project includes a **Flask-based web application** that serves predictions through a simple user interface.

The application demonstrates how modern machine learning techniques can support investors and traders in making better-informed investment decisions by analyzing trends, returns, risk, and future price movements.

---

## Team Members (Group 9)

* Bahareh Arghavani Nobar
* Devnath Reddy Motati
* Vijitha Pyeta Gouda Kake
* Naga Venkata Sai Teja Keerty

---

## Problem Statement

Predicting future stock prices to assist investors and traders in:

* Making better-informed investment decisions
* Managing financial risk
* Potentially improving overall returns

---

## Objectives

* Develop a machine learning–based stock price prediction system
* Apply time-series modeling using LSTM networks
* Perform exploratory data analysis (EDA) and visualization
* Evaluate prediction accuracy using standard regression metrics
* Deploy the trained model via a web application

---

## Methodology (CRISP-DM Framework)

### 1. Business Understanding

Investors require reliable and accurate tools to forecast stock prices in order to identify opportunities and mitigate risks in highly volatile markets.

### 2. Data Understanding

* Data Source: **Yahoo Finance**
* Data Access: `yfinance` Python library
* Data includes: Open, High, Low, Close prices and Volume

### 3. Data Analysis

Key analytical questions addressed:

* How does stock price change over time?
* What is the average daily return?
* What are the moving averages over different periods?
* How correlated are different stocks?
* What level of risk is associated with a stock?
* How accurately can an LSTM predict future closing prices?

### 4. Data Preparation

* Data cleaning and handling missing values
* Feature selection (primarily Open and Close prices)
* Data normalization and scaling
* Train–test split for time-series modeling

### 5. Modeling

* Model Type: **Long Short-Term Memory (LSTM)** neural network
* Architecture:

  * One or more LSTM layers
  * Dense layers
  * Linear activation output layer
* Loss Function: Mean Squared Error (MSE)
* Optimizer: Adam (or equivalent)

### 6. Evaluation

Model performance evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

### 7. Deployment

* Framework: **Flask**
* Model serialized using `pickle`
* Web interface for user input and prediction output
* Deployment-ready for cloud platforms such as **AWS** or **Azure**

---

## Repository Structure

```
Stock_Market_Prediction/
│
├── README.md                     # Project documentation
├── app.py                        # Flask application
├── Stock_Prediction_.ipynb       # Jupyter notebook (EDA + LSTM model)
├── model.pkl                     # Trained LSTM model
├── home.html                     # Homepage template
├── result.html                   # Prediction result page
├── error.html                    # Error handling page
├── Stock Market Prediction.pptx  # Project presentation
├── Stock Market Prediction_Report.docx # Technical report
```

---

## Application Workflow

1. User provides stock-related input via the web interface
2. Flask application loads the trained LSTM model
3. Input data is preprocessed and scaled
4. Model generates future stock price predictions
5. Results are displayed on the web UI

---

## Technologies Used

### Programming & Libraries

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* TensorFlow / Keras
* yfinance
* Scikit-learn

### Web & Deployment

* Flask
* HTML/CSS
* Pickle (model serialization)
* Cloud-ready (AWS / Azure)

---

## Results & Conclusion

* LSTM models demonstrated reasonable accuracy in predicting future stock prices
* Performance varies depending on stock volatility and market conditions
* Accuracy can be improved by:

  * Hyperparameter tuning
  * Adding more historical data
  * Exploring advanced architectures

While predictions are informative, real-world investment decisions should also consider external economic and market factors.

---


Email: [dmota1@unh.newhaven.edu](mailto:dmota1@unh.newhaven.edu)
