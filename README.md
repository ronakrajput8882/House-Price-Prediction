# 🏠 House Price Prediction

A machine learning project that predicts residential house sale prices using **Linear Regression** based on key property features.

---

## 📂 Dataset

- **File:** `HousePricePrediction.csv`
- **Total Records:** 2,919 rows
- **Target Variable:** `SalePrice` (house sale price in USD)

### 📋 Features Used

| Column | Description |
|---|---|
| `MSSubClass` | Type of dwelling involved in the sale |
| `MSZoning` | General zoning classification |
| `LotArea` | Lot size in square feet |
| `LotConfig` | Lot configuration |
| `BldgType` | Type of building |
| `OverallCond` | Overall condition rating of the house |
| `YearBuilt` | Original construction year |
| `YearRemodAdd` | Remodel year |
| `Exterior1st` | Exterior covering on house |
| `BsmtFinSF2` | Finished basement area (sq ft) |
| `TotalBsmtSF` | Total basement area (sq ft) |
| `SalePrice` | ✅ Target — Sale price of the house |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python | Core programming language |
| pandas | Data loading, cleaning, manipulation |
| NumPy | Numerical operations |
| seaborn | Data visualization |
| scikit-learn | ML model, preprocessing, evaluation |
| Jupyter Notebook | Development environment |

---

## 🔄 Project Workflow

```
1. Load Data
      ↓
2. Data Cleaning       → Handle nulls (fill SalePrice with mean, drop remaining)
      ↓
3. Encoding            → One-hot encode: MSZoning, LotConfig, BldgType, Exterior1st
      ↓
4. Train/Test Split    → 80% train, 20% test (random_state=0)
      ↓
5. Feature Scaling     → StandardScaler on train and test sets
      ↓
6. Model Training      → Linear Regression (scikit-learn)
      ↓
7. Evaluation          → R², MAE, RMSE, MAPE
```

---

## 📊 Model Results

| Metric | Score |
|---|---|
| **R² Score** | 0.374 |
| **MAE** | ~30,829 |
| **RMSE** | ~41,138 |
| **MAPE** | ~18.7% |

> ℹ️ The baseline Linear Regression model explains ~37% of the variance in sale prices. Future improvements could include Random Forest or XGBoost for better accuracy.

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/ronakrajput8882/house-price-prediction.git
cd house-price-prediction
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch the notebook
```bash
jupyter notebook HousePricePred.ipynb
```

### 4. Run all cells
In Jupyter: **Kernel → Restart & Run All**

---

## 📦 Requirements

```
pandas
numpy
seaborn
scikit-learn
jupyter
```

---

## 🔮 Future Improvements

- Try **Random Forest** and **XGBoost** for higher accuracy
- Add more features (bedrooms, bathrooms, garage, etc.)
- Hyperparameter tuning with GridSearchCV
- Deploy as a web app using Streamlit or Flask

---

## 👤 Author

**Ronaksinh Rajput**
- GitHub: [@ronakrajput8882](https://github.com/ronakrajput8882)
- LinkedIn: [ronaksinh-rajput8882](https://linkedin.com/in/ronaksinh-rajput8882)
