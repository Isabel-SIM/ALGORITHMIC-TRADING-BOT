# Algorithmic Trading Bot with Machine Learning

## Overview

In this project, I have developed an algorithmic trading bot that utilizes machine learning to automate trade decisions. The aim is to enhance trading strategies and adapt to evolving market conditions. This project combines financial Python programming and machine learning to create a dynamic trading system.

## Background

As a financial advisor at a top-tier financial advisory firm, we recognize the importance of staying competitive in a rapidly evolving market. To maintain our edge, we are enhancing our existing algorithmic trading systems. While speed has been our advantage, we aim to improve adaptability to new data using machine learning algorithms.

## Existing Model Data

Before diving into the details of the project, let's take a look at the performance of our existing models:

### Model ONE

- Short Window: 4
- Long Window: 100
- Date Offset months: 3

**Results:**
- Precision: 0.43
- Recall: 0.04
- F1-Score: 0.07
- Accuracy: 0.55

[![Model ONE Returns Plot](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot.png?raw=true)](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot.png?raw=true)

### Model TWO

- Short Window: 10
- Long Window: 150
- Date Offset months: 6

**Results:**
- Precision: 0.38
- Recall: 0.01
- F1-Score: 0.01
- Accuracy: 0.56

[![Model TWO Returns Plot](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot_2.png?raw=true)](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot_2.png?raw=true)

### Model THREE

- Short Window: 30
- Long Window: 100
- Date Offset months: 4

**Results:**
- Precision: 0.44
- Recall: 0.04
- F1-Score: 0.07
- Accuracy: 0.56

[![Model THREE Returns Plot](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot_3.png?raw=true)](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot_3.png?raw=true)

### Model FOUR

- Short Window: 40
- Long Window: 200
- Date Offset months: 5

**Results:**
- Precision: 0.45
- Recall: 0.31
- F1-Score: 0.37
- Accuracy: 0.53

[![Model FOUR Returns Plot](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot_4.png?raw=true)](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/returns_plot_4.png?raw=true)

## Model Analysis

### Q1: Impact of Training Window

The impact of increasing or decreasing the training window:

- Increasing the training window provides more historical data for the model to learn from, enabling it to capture longer-term trends and patterns. This often leads to improved performance, as observed in Model TWO and Model FOUR, which had longer training windows and achieved higher precision, recall, and F1-scores.
- Decreasing the training window limits the amount of historical data available for the model to learn from, potentially reducing its ability to capture complex relationships and make accurate predictions. This is evident in Model ONE and Model THREE, which had shorter training windows and lower performance metrics.

### Q2: Impact of SMA Window Sizes

The impact of increasing or decreasing the SMA windows:

- Increasing the short window allows the model to consider a larger number of recent data points when calculating the SMA, capturing short-term trends more effectively. This can improve performance, as seen in Model THREE compared to Model ONE.
- Increasing the long window enables the model to consider a larger number of historical data points when calculating the SMA, helping it capture longer-term trends and broader market movements. This can enhance performance, as demonstrated in Model FOUR compared to Model TWO.

### Q3: Evaluation of New Machine Learning Classifier (ADABOOST)

#### Model ADABOOST

**Results:**
- Precision: 0.44
- Recall: 0.08
- F1-Score: 0.13
- Accuracy: 0.55

[![Model ADABOOST Returns Plot](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/adaboost_plot.png?raw=true)](https://github.com/isabelsimundic/WEEK-FOURTEEN-HOMEWORK/blob/main/CODE/adaboost_plot.png?raw=true)

Based on this analysis, the new model performs better than the baseline model in terms of precision and F1-score but worse in terms of recall and accuracy. When compared to the tuned trading algorithms (Models Two, Three, and Four), the new model generally performs worse across different metrics, except for precision.

By combining algorithmic trading and machine learning, this project aims to create a sophisticated trading bot that adapts to evolving markets, ultimately enhancing our firm's competitive advantage in the financial industry.

