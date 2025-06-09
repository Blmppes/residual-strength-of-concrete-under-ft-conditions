# Application of Advanced Gradient Boosting Models for Predicting the Residual Strength of Concrete under Freeze–Thaw Conditions

This project aims to predict the Decreased Compressive Strength (DCS) of concrete under FTC (Freeze–Thaw Cycles) using various machine learning techniques: Support Vector Regression (SVM), Random Forest (RF), and Artificial Neural Network (ANN), XG Boost, CatBoost.

The models have been trained and tuned based on a scientific dataset and evaluated using MAE, RMSE, and R² metrics. The objective is to outperform results from prior studies and offer reproducible experiments.

## 📁 Files Overview
- ann_model.py         → Train and evaluate the ANN model.
- svm_model.py         → Train and evaluate the SVM model.
- rf_model.py          → Train and evaluate the Random Forest model.
- requirements.txt     → Fixed-version environment to guarantee reproducibility.
- ann_model.keras      → Saved ANN model in Keras HDF5 format.
- svm_model.pkl        → Saved SVM model using `joblib`.
- rf_model.pkl         → Saved Random Forest model using `joblib`.

## ✅ Reproduce Results

1. **Install dependencies**:
```bash
pip install -r requirements.txt
2. **Train models**:
You can run the corresponding *.py files to retrain models from scratch.
3. **Load pretrained models**:
Load ANN:
from tensorflow.keras.models import load_model
model = load_model("ann_model.keras")
Load SVM or RF:
import joblib
svm_model = joblib.load("svm_model.pkl")
rf_model = joblib.load("rf_model.pkl")