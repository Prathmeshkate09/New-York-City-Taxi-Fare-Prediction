# New-York-City-Taxi-Fare-Prediction

This project predicts taxi fares in New York City using machine learning techniques based on historical ride data. The trained model is saved as `New_York_City_Taxi_Fare_Prediction.pkl`.

---

## 📌 Project Overview

- **Goal**: Predict the fare amount for NYC taxi rides based on pickup/dropoff location, time, and passenger count.
- **Model Used**: XGBoost Regressor
- **Dataset**: NYC Taxi Fare dataset (from [Kaggle](https://www.kaggle.com/c/new-york-city-taxi-fare-prediction/data))
- **Saved Model**: `New_York_City_Taxi_Fare_Prediction.pkl` using `joblib`

---

## 📁 Project Structure
New_York_City_Taxi_Fare_Prediction/
│
├── model/                          # Trained machine learning model
│   └── New_York_City_Taxi_Fare_Prediction.pkl
│
├── notebooks/                      # Jupyter Notebooks for EDA & training
│   └── ALLINONE.ipynb              # Combined notebook (EDA + preprocessing + model)
│
├── requirements.txt                # Python dependencies
└── README.md                       # Project documentation



---

## ⚙️ Features Used

- Pickup and dropoff latitude & longitude
- Pickup datetime (with feature engineering)
- Passenger count
- Distance calculation (Haversine formula)

---

## 🛠️ How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Prathmeshkate09/New_York_City_Taxi_Fare_Prediction.git
   cd New_York_City_Taxi_Fare_Prediction

   Install Dependencies:

pip install -r requirements.txt



