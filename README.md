# Implementation of Random Forest Algorithm for Weather Prediction
## AIM:
To write a program to predict daily temperature , PM2.5 pollution level and Energy based on environmental sensor data using Random Forest Algorithm.

## Problem Statement and Dataset



## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required libraries and create the weather dataset.
2. Split the dataset into input and output variables.
3. Train the Random Forest model using training data.
4. Predict temperature, PM2.5, and energy values and display the results.

## Program:
```
/*
Program to implement the Random Forest Algorithm to predict daily temperature , PM2.5 pollution level and Energy based on environmental sensor data.
Developed by: VASHMITHA V
RegisterNumber:212225240180
# Import libraries
import pandas as pd
from sklearn.ensemble import RandomForestRegressor

# Create dataset
data = {
    'Humidity': [30, 40, 50, 60, 70],
    'WindSpeed': [5, 7, 9, 11, 13],
    'Temperature': [25, 28, 30, 35, 40],
    'PM25': [50, 55, 60, 70, 80],
    'Energy': [100, 120, 140, 160, 180]
}

# Create DataFrame
df = pd.DataFrame(data)

# Input features
X = df[['Humidity', 'WindSpeed']]

# Output targets
y = df[['Temperature', 'PM25', 'Energy']]

# Create model
model = RandomForestRegressor(n_estimators=10, random_state=0)

# Train model
model.fit(X, y)

# Predict values
prediction = model.predict([[45, 8]])

# Display output
print("Predicted Temperature:", prediction[0][0])
print("Predicted PM2.5:", prediction[0][1])
print("Predicted Energy:", prediction[0][2])
*/
```

## Output:
<img width="382" height="71" alt="Screenshot 2026-05-13 091529" src="https://github.com/user-attachments/assets/46602343-6149-4356-a2ee-eb827f3134ed" />


## Result:
