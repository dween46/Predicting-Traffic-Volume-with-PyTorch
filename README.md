# 🚗 Traffic Volume Prediction using Deep Learning


This project is a part of a DataCamp assignment where the goal is to develop a time-series model that predicts hourly traffic volume on an interstate highway using deep learning techniques.

Predicting traffic volume can be challenging due to its fluctuation and dependence on time and external factors like weather and holidays. This project demonstrates how deep learning can help identify abstract patterns and boost predictability.

## 📈 Problem Statement

The task is to build a deep learning model that predicts the `traffic_volume` (number of vehicles passing at a specific location) using various features like weather, time, and holidays.

Such models can be valuable in:
- Reducing road congestion
- Designing more efficient roads and intersections
- Improving commute planning
- Enhancing traffic safety

## 📊 Dataset

The dataset is sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/) and includes hourly records of traffic volume on Interstate I-94 in Minnesota, USA.

### Available Files
- `train_scaled.csv`
- `test_scaled.csv`

### Features

| Feature                         | Type        | Description                                                  |
|----------------------------------|-------------|--------------------------------------------------------------|
| `temp`                           | Numeric     | Average temperature (Kelvin)                                 |
| `rain_1h`, `snow_1h`             | Numeric     | Precipitation in mm during the hour                          |
| `clouds_all`                     | Numeric     | Percentage of cloud cover                                    |
| `date_time`                      | DateTime    | Local time (CST)                                             |
| `holiday_` (11 columns)          | Categorical | National and regional US holidays including MN State Fair    |
| `weather_main_` (11 columns)     | Categorical | Short weather description                                    |
| `weather_description_` (35 cols) | Categorical | Detailed weather description                                 |
| `hour_of_day`, `day_of_week`, `day_of_month`, `month` | Numeric | Time components extracted from `date_time` |
| `traffic_volume`                 | Numeric     | Target variable: hourly westbound traffic volume             |

## 🧠 Methodology

- Exploratory Data Analysis (EDA)
- Feature Engineering and Encoding
- Data Normalization
- Time-Series Modeling with Deep Learning (LSTM/RNN)
- Evaluation of model performance using MAE/MSE/RMSE

## 📦 Requirements

- Python 3.x
- pytorch / Keras
- NumPy / Pandas / Matplotlib / Seaborn
- Scikit-learn

Install dependencies with:

```bash
pip install -r requirements.txt
