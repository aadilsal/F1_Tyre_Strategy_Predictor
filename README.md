# # 🏎️ F1 Tyre Strategy & Performance Predictor

A data-driven predictive analytics project designed to forecast **Formula 1 race tyre strategies and driver performance outcomes**. This project combines multiple machine learning models to help race strategists, analysts, and motorsport enthusiasts gain insights into potential race outcomes based on historical race data and grid positions.

---

## 📊 Project Overview

This tool predicts:
- The number of **pit stops** a driver is likely to make during a race.
- The likelihood of a driver achieving the **Fastest Lap**.
- The probability of a driver becoming the **Race Winner** based on their starting grid position and other race factors.

---

## 🔍 Machine Learning Models Used

1️⃣ **Tyre Strategy Prediction Model**  
- Classification model predicting the number of pit stops per driver.  
- Input Features:  
  - Average pit lap  
  - Last pit lap  
  - Average pit stop time  
  - Circuit-specific tyre compound availability  

2️⃣ **Fastest Lap Candidate Model**  
- Classification model using **grid position** to predict potential fastest lap candidates.

3️⃣ **Race Winner Prediction Model**  
- Classification model forecasting the probability of a driver winning the race based on their **starting grid position**.

---

## 🛠️ How It Works

The project takes in driver and race-specific inputs such as:
- Average and last pit lap numbers
- Average pit stop times
- Circuit-specific tyre compound options
- Driver's grid position

and generates an output like:

```python
{
  'Driver': 'Lando Norris',
  'Predicted Pit Strategy (stops)': 2,
  'Tyre Compounds Used': [2, 3],
  'Fastest Lap Candidate': 'Lando Norris',
  'Winner Candidate': None
}
