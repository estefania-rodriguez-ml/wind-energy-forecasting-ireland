# Short-Term Wind Energy Forecasting in Ireland

## Project Overview
Ireland aims to generate 80% of electricity from renewable sources by 2030, with wind energy as a key component. However, its variability creates challenges for grid stability and energy planning.

This project develops and compares statistical and machine learning models to improve short-term wind energy forecasting.

---

## Objectives
- Build forecasting models for wind energy production
- Compare performance across different modelling approaches
- Analyse how prediction accuracy changes across time horizons

---

## Models Used
- SARIMA (statistical time series model)
- Random Forest (machine learning)
- LSTM (deep learning)

---

## Methodology
The project follows the CRISP-DM framework:
- Business Understanding
- Data Understanding
- Data Preparation
- Modelling
- Evaluation

Key steps included:
- Time series resampling (15-min → daily)
- Handling missing and invalid values
- Feature engineering using lag variables and sliding windows
- Model evaluation using MAE and RMSE across multiple horizons (3, 5, 7 days)

---

## Dataset
- Source: EirGrid (Ireland’s Transmission System Operator)
- Frequency: 15 minutes
- Period: 2013–2025

⚠️ The dataset is not included due to access restrictions.

---

## Results
- Random Forest achieved the best overall performance for short-term forecasts
- LSTM captured temporal dependencies but required higher computational cost
- SARIMA provided a strong statistical baseline but struggled with non-linear patterns

---

## Conclusion
Machine learning models outperform traditional statistical approaches in capturing complex wind generation patterns. However, Random Forest offers the best trade-off between accuracy and computational efficiency.

---

## Future Work
- Incorporate meteorological variables (wind speed, direction)
- Develop multivariate LSTM models
- Improve data granularity using wind farm-level data

---

## Tools & Technologies
- Python (Pandas, NumPy)
- Scikit-learn
- TensorFlow / Keras
- Matplotlib / Seaborn

---

## Project Structure
- `wind_energy_forecasting.ipynb` → main notebook