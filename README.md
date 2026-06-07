# Socbiz_Openproject
# Agentic AI for Dynamic EV Charging Tariff Optimization

## Overview

As EV adoption increases, fixed charging tariffs often lead to peak-hour congestion, low off-peak utilization, and inefficient revenue generation. This project proposes an Agentic AI framework that forecasts EV charging demand, recommends dynamic tariffs, and continuously monitors system performance.

## Problem Statement

Develop an intelligent pricing engine that:

* Predicts EV charging demand
* Optimizes charging tariffs in real time
* Improves charger utilization
* Increases charging station revenue
* Supports continuous monitoring and feedback

## Datasets

### ACN-Data (Caltech & JPL)

* 31,900+ charging sessions
* Energy delivered
* Session duration
* Station information
* User behavior patterns

### UrbanEV Dataset

* 247 charging stations
* Occupancy data
* Charging volume
* Charging duration
* Electricity pricing

## Project Architecture

EV Charging Data
↓
Demand Prediction Agent (XGBoost)
↓
Dynamic Tariff Pricing Agent
↓
Monitoring & Learning Agent
↓
Revenue & Utilization Optimization

## Methodology

### 1. Data Preprocessing

* Data cleaning
* Missing value handling
* Datetime conversion
* Feature engineering
* Hourly demand aggregation

### 2. Demand Prediction Agent

Model: XGBoost Regressor

Features:

* Lag Features
* Rolling Statistics
* Time Features
* Cyclic Features

### 3. Dynamic Tariff Pricing Agent

Pricing strategies evaluated:

* Rule-Based Pricing
* Aggressive Pricing
* Percentile-Based Pricing

### 4. Monitoring & Learning Agent

Monitors:

* Revenue
* Utilization
* Congestion
* Pricing efficiency

## Results

| Metric              | Value   |
| ------------------- | ------- |
| Sessions Analyzed   | 31,900+ |
| R² Score            | 0.738   |
| RMSE                | 3.22    |
| MAE                 | 2.03    |
| Revenue Gain        | 22.95%  |
| Average Utilization | 70.17%  |

## Key Insights

* Peak charging demand occurs between 13:00–16:00.
* Dynamic pricing significantly outperforms fixed pricing.
* Percentile-based pricing achieved the highest revenue improvement.
* Agent-based monitoring enables continuous policy evaluation.

## Repository Structure

```text
├── Final_Notebook.ipynb
├── Presentation.pdf
├── README.md
├── figures/
└── data/
```

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* XGBoost

## Conclusion

The proposed Agentic AI framework successfully forecasts EV charging demand and optimizes tariff decisions. The system achieved a 22.95% increase in revenue while maintaining healthy charger utilization, demonstrating the effectiveness of AI-driven pricing strategies for EV charging infrastructure.
