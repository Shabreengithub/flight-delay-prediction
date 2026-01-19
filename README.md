# Flight Delay Prediction – Plight to Right ✈️

Machine learning project to predict flight departure delays using 10 years of U.S. flight and weather data. The project applies data preprocessing, feature engineering, time-series analysis, and XGBoost regression to build a predictive model for aviation delay management.

---

## 📌 Project Overview

This project analyzes flight departure data from major U.S. airports (LAX, JFK, ORD, DFW) to identify delay patterns and understand the impact of weather on flight operations. The goal is to build a machine learning model that predicts flight delays and supports data-driven decision-making for airlines and passengers.

---

## 📊 Dataset Features

- loan_size → *(Not applicable here, remove if unused)*  
- **Flight Data:** Departure time, airport, airline, delay metrics  
- **Weather Data:** Temperature, humidity, wind speed, precipitation, visibility  
- **Target Variable:** Total flight departure delay  

*(Flight and weather datasets were merged and time-zone normalized for accurate alignment.)*

---

## ⚙️ Methodology

- Collected flight data from the Bureau of Transportation Statistics  
- Collected weather data from the Iowa Mesonet  
- Performed:
  - Data cleaning and missing value handling  
  - Time-zone normalization  
  - Outlier detection using Local Outlier Factor (LOF)  
  - Feature engineering (humidity, wind chill, heat index, rolling delay trends)  
- Trained and evaluated:
  - XGBoost  
  - LightGBM  
  - Random Forest Regressor  
- Selected **XGBoost** as the best-performing model based on RMSE evaluation  

---

## 📈 Results

- XGBoost achieved the lowest RMSE among tested models  
- Weather conditions showed significant correlation with flight delays  
- Model provides predictive insights for operational planning and delay management  

---

## 🛠️ Tech Stack

Python • Pandas • Scikit-learn • XGBoost • LightGBM • Feature Engineering • Time-Series Analysis • Data Visualization

---

## 🏆 Conclusion

This project demonstrates how machine learning and weather analytics can effectively predict flight delays. The study highlights the importance of data quality, feature engineering, and model evaluation in building reliable predictive systems for the aviation industry.

---

## 🚀 Future Improvements

- Integrate real-time weather data for live delay predictions  
- Deploy model as a REST API using FastAPI  
- Build an interactive dashboard for visualization  

---

## 📂 Repository Contents

- `Flight_Delay_Prediction.ipynb` → Jupyter notebook with full analysis and model training  
- `Flight Delay Prediction Final Report.pdf` → Detailed project report  
- `README.md` → Project documentation  

---

## 🔗 Project Link

GitHub Repository:  
https://github.com/Shabreengithub/flight-delay-prediction

