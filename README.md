# SCT_ML_1
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
