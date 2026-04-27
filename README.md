## Crypto Currency Price Prediction

## Overview

This project implements cryptocurrency price prediction for Bitcoin (BTC), Litecoin (LTC), and Ethereum (ETH) using multiple machine learning approaches including Linear Regression, LSTM Neural Networks, and Facebook Prophet.


## Models Implemented


## 1. Linear Regression
   
Features used: Open, High, Low, Volume

Target: Close price

Training/Test split: 70/30

Prediction horizon: 40 days ahead


## 2. LSTM (Long Short-Term Memory)

Architecture:

LSTM layer (64 units)

LeakyReLU activation (alpha=0.5)

Dropout (0.1)

Dense output layer (1 unit)

Sequence length: 5 days of historical data

Optimizer: Adam (learning_rate=0.0001)

Loss function: MSE

Epochs: 250

Batch size: 5


## 3. Prophet (Facebook)

Time series forecasting with daily seasonality

365-day forecast horizon


## Results

## Linear Regression Evaluation

## Metric	Value

MSE 	 5.43e-08

MAE	   0.000233


## LSTM Training

Final validation loss: ~1.08e-04

Training loss: ~4.55e-04


## Data Sources

The models were trained on historical price data for:

BTC-USD

LTC-USD

ETH-USD

Data includes daily Open, High, Low, Close, Volume and Date columns.


## Dependencies

pandas

numpy

matplotlib

seaborn

scikit-learn

tensorflow/keras

prophet

cmdstanpy


## Usage

Load the cryptocurrency CSV data files

Preprocess and normalize the data

Choose a model (Linear Regression, LSTM, or Prophet)

Train the model on historical data

Generate predictions and visualize results


## Key Features

Data normalization using MinMaxScaler

Time series data preparation for LSTM

Visualization of actual vs predicted prices

Multiple cryptocurrency support


## Model Performance Notes

Linear Regression shows reasonable performance with low error metrics

LSTM achieves stable convergence with low validation loss

Prophet provides interpretable time series forecasts with seasonality components
