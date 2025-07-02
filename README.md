# 🚖 New York City Taxi Fare Prediction

This machine learning project predicts taxi fare amounts in New York City based on ride details such as pickup/dropoff locations, time, and number of passengers.  
The final model is saved as `New_York_City_Taxi_Fare_Prediction.pkl` and can be reused for inference or deployment.

---

## 📌 Project Overview

- **📊 Objective**: Predict the fare amount for a taxi ride in NYC.
- **🔧 ML Model**: XGBoost Regressor
- **📂 Model File**: `model/New_York_City_Taxi_Fare_Prediction.pkl`
- **📁 Notebook**: `notebooks/ALLINONE.ipynb` contains EDA, preprocessing, training, and model saving
- **🗃️ Data**: Based on the public [NYC Taxi Fare dataset](https://www.kaggle.com/competitions/new-york-city-taxi-fare-prediction)

---

## 📁 Project Structure

New_York_City_Taxi_Fare_Prediction/
│
├── model/
│ └── New_York_City_Taxi_Fare_Prediction.pkl # Trained model
│
├── notebooks/
│ └── ALLINONE.ipynb # EDA + Training Notebook
│
├── requirements.txt # Python dependencies
└── README.md # Project documentation


---

## ⚙️ Features Used

- Pickup and dropoff **latitude & longitude**
- **Haversine distance** calculation between pickup and dropoff
- **Datetime features**: day, hour, weekday, month
- Passenger count

---

## 🔍 How to Use the Model

```python
import joblib

# Load the saved model
model = joblib.load('model/New_York_City_Taxi_Fare_Prediction.pkl')

# Example input: [pickup_lat, pickup_long, drop_lat, drop_long, passenger_count, distance]
sample_input = [[40.761432, -73.979815, 40.651311, -73.880333, 1, 12.2]]

# Predict fare
fare = model.predict(sample_input)
print(f"Predicted Fare: ${fare[0]:.2f}")

Installation
pip install -r requirements.txt

