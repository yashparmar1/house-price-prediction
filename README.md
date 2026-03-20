# House Price Prediction Model
> Regression project comparing 4 machine learning models — XGBoost achieved best performance with **83.01% R² score**.

## Overview
This project develops and compares multiple machine learning regression models to predict housing prices using the California Housing dataset. It demonstrates structured data preprocessing, model comparison, hyperparameter awareness, and performance evaluation.

## Real Results — Model Comparison
| Model | R² Score |
|-------|----------|
| Decision Tree | 61.28% |
| Gradient Boosting | 77.57% |
| Random Forest | 80.53% |
| **XGBoost** | **83.01%** ← best model |

Linear Regression baseline: R² = 0.576, MAE = 0.533, MSE = 0.556

## Project Workflow
1. **Data Loading** — used California Housing dataset via scikit-learn (20,640 records, 8 features)
2. **Data Exploration** — inspected feature distributions, data types, and first rows
3. **Preprocessing** — split 80/20 train/test; applied StandardScaler normalisation to all features
4. **Baseline Model** — trained Linear Regression; achieved R²=0.576, MAE=0.533
5. **Model Comparison** — trained and evaluated Decision Tree, Random Forest, Gradient Boosting, and XGBoost
6. **Model Saving** — saved best model using joblib for reuse

## Dataset Features
| Feature | Description |
|---------|-------------|
| MedInc | Median income in block group |
| HouseAge | Median house age in block group |
| AveRooms | Average number of rooms per household |
| AveBedrms | Average number of bedrooms per household |
| Population | Block group population |
| AveOccup | Average household occupancy |
| Latitude | Block group latitude |
| Longitude | Block group longitude |
| **Price** | **Target: median house value (in $100,000s)** |

## Tech Stack
- **Language:** Python 3
- **Libraries:** Pandas, NumPy, scikit-learn, XGBoost, joblib, Matplotlib
- **Environment:** Jupyter Notebook (Anaconda)

## Key Skills Demonstrated
- Data preprocessing and feature scaling (StandardScaler)
- Comparative model evaluation across 4 algorithms
- Regression metrics: MAE, MSE, R-squared
- Ensemble methods: Random Forest, Gradient Boosting, XGBoost
- Model persistence with joblib

## How to Run
```bash
git clone https://github.com/yashparmar1/house-price-prediction.git
cd house-price-prediction
pip install pandas numpy scikit-learn xgboost joblib matplotlib jupyter
jupyter notebook house_price_prediction.ipynb
```

## Author
**Yashkumar Parmar**
MSc Data Science — Middlesex University London (2026)
[LinkedIn](https://www.linkedin.com/in/yashkumar-parmar-7752b8238) · [GitHub](https://github.com/yashparmar1)

