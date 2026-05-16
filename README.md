# 🏠 House Price Prediction using Linear Regression

This project implements a **Linear Regression Model** to predict house prices using:

- Square Footage (`GrLivArea`)
- Number of Bedrooms (`BedroomAbvGr`)
- Number of Full Bathrooms (`FullBath`)
- Number of Half Bathrooms (`HalfBath`)

The model is trained using the **House Prices Dataset** and evaluated using regression metrics.

---

# 📂 Dataset

Dataset Used:
- `train.csv`
- `test.csv`

Dataset Shape:

```text
Train shape: (1460, 81)
Test shape : (1459, 80)
```

---

# 🚀 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn

---

# 📊 Features Used

| Feature | Description |
|---|---|
| GrLivArea | Above ground living area square feet |
| BedroomAbvGr | Number of bedrooms above ground |
| FullBath | Number of full bathrooms |
| HalfBath | Number of half bathrooms |

Target Variable:
- `SalePrice`

---

# 🧠 Machine Learning Model

Model Used:
- **Linear Regression**

The model learns relationships between selected house features and house prices.

---

# ⚙️ Project Workflow

1. Load the dataset
2. Explore dataset shape and sample rows
3. Select important features
4. Check missing values
5. Split data into training and validation sets
6. Train Linear Regression model
7. Predict house prices
8. Evaluate performance

---

# 📄 First 5 Rows of Dataset

```text
   Id  MSSubClass MSZoning  ...  SaleType  SaleCondition SalePrice
0   1          60       RL  ...        WD         Normal    208500
1   2          20       RL  ...        WD         Normal    181500
2   3          60       RL  ...        WD         Normal    223500
3   4          70       RL  ...        WD        Abnorml    140000
4   5          60       RL  ...        WD         Normal    250000

[5 rows x 81 columns]
```

---

# 🔍 Missing Values in Selected Features

```text
GrLivArea       0
BedroomAbvGr    0
FullBath        0
HalfBath        0
SalePrice       0
dtype: int64
```

---

# 📈 Validation Metrics

```text
MAE  : $36,018.56
RMSE : $53,018.33
R²   : 0.6335
```

## 📌 Metric Explanation

### ✅ MAE (Mean Absolute Error)
Average absolute difference between predicted and actual prices.

### ✅ RMSE (Root Mean Squared Error)
Measures prediction accuracy with higher penalty for large errors.

### ✅ R² Score
Shows how well the model explains the variation in house prices.

---

# 📊 Model Coefficients

```text
     Feature   Coefficient
   GrLivArea  53329.038949
    FullBath  16863.945379
    HalfBath   2304.622887
BedroomAbvGr -21483.654769
```

Intercept:

```text
181,441.54
```

---

# 💻 Complete Output

```text
PS C:\Users\reddy\OneDrive\Desktop\HousePrice> python -u "c:\Users\reddy\OneDrive\Desktop\HousePrice\house_price_model.py"

Train shape: (1460, 81)
Test shape : (1459, 80)

First 5 rows:
   Id  MSSubClass MSZoning  ...  SaleType  SaleCondition SalePrice
0   1          60       RL  ...        WD         Normal    208500
1   2          20       RL  ...        WD         Normal    181500
2   3          60       RL  ...        WD         Normal    223500
3   4          70       RL  ...        WD        Abnorml    140000
4   5          60       RL  ...        WD         Normal    250000

[5 rows x 81 columns]

Missing values in selected features:
GrLivArea       0
BedroomAbvGr    0
FullBath        0
HalfBath        0
SalePrice       0
dtype: int64

── Validation Metrics ──────────────────
  MAE  : $36,018.56
  RMSE : $53,018.33
  R²   : 0.6335
────────────────────────────────────────

Model Coefficients:
     Feature   Coefficient
   GrLivArea  53329.038949
    FullBath  16863.945379
    HalfBath   2304.622887
BedroomAbvGr -21483.654769

Intercept: 181,441.54
```

---

# 📁 Project Structure

```text
HousePrice/
│
├── train.csv
├── test.csv
├── house_price_model.py
└── README.md
```

---

# 🎯 Future Improvements

- Add more house features
- Improve accuracy using advanced models
- Perform feature engineering
- Deploy using Flask or Streamlit

---
