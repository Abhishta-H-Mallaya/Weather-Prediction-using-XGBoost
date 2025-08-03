# 🌫️ Air Quality Prediction using XGBoost and Arduino Sensor Data

## 📌 Overview
This project focuses on real-time **air quality prediction** using the **XGBoost** machine learning algorithm trained on data collected from Arduino-based sensors. It merges hardware-based environmental sensing with robust machine learning for accurate forecasting of air quality, particularly **PM2.5**, along with **temperature**, **humidity**, and **pressure**.

---

## 🛠️ Hardware Setup & Data Collection

- **Arduino UNO** – Central microcontroller interfacing with sensors.
- **Adafruit BME280** – Captures **temperature**, **humidity**, and **atmospheric pressure**.
- **Grove HM3301 Dust Sensor** – Measures **PM2.5 particulate matter**, a key air pollution indicator.
- Data is logged via USB/serial connection and formatted into structured time series data.

---

## 🔁 Process Flow

1. **Data Collection**
   - Sensors capture environmental conditions in real-time and stream data to a connected device.

2. **Preprocessing**
   - Missing values handled.
   - Features generated using rolling statistics (e.g., moving averages over days or weeks).

3. **Train/Test Split**
   - Historic data used for training.
   - Recent data reserved for testing to preserve time-based integrity.

4. **Model Training with XGBoost**
   - Leverages gradient boosting trees to learn correlations between environmental features and PM2.5 levels.

5. **Evaluation Metrics**
   - Accuracy measured using:
     - Mean Absolute Error (MAE)
     - Mean Squared Error (MSE)
     - Coefficient of Determination (R² Score)

6. **Real-Time Optimization**
   - The model can be updated incrementally as new sensor data is collected, improving performance over time.

---

## 📊 Results

- Accurate predictions for air quality using PM2.5 and related atmospheric parameters.
- Graphs illustrating **actual vs. predicted** values.
- Feature importance insights (e.g., temperature or humidity's effect on PM2.5).

---

## 💡 Features

- Integration of **hardware and software** for real-world application.
- Real-time predictions based on **sensor-collected data**.
- Built using **XGBoost**, known for high accuracy and performance in regression problems.
- Scalable architecture: Can be extended to AQI prediction or more sensors.

---

## 🧪 Tech Stack

- **Hardware**: Arduino UNO, BME280, Grove HM3301
- **Languages**: Python
- **Libraries**: 
  - `xgboost`
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `scikit-learn`

---

## 📂 Project Structure

- `WEARTHER_PREDICTION.ipynb` – Core notebook: data cleaning, model training, evaluation
- `DATA SET-MATH.xlsx` – Collected dataset
- `README.md` – Documentation

---

## 👥 Contributors

Developed by:

- [Kanishka S J](https://github.com/kanishkasj)
- [Abhishta H Mallaya](https://github.com/Abhishta-H-Mallaya)

---
        
