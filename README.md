# Bangkok Airbnb — Market Analysis & Price Prediction
### EDA → Clustering → Price Prediction Pipeline

Full data science pipeline on 23,000+ Bangkok Airbnb listings using 
[Inside Airbnb](http://insideairbnb.com) data (September 2025).

---

## Key Findings

**EDA**
- Accommodation size is the dominant price driver — each additional 
  guest capacity increases nightly price by ~19%
- Central districts (Parthum Wan, Bang Rak) price 3–4× higher than 
  peripheral areas — location prestige matters more than listing volume
- Superhosts respond to 99.1% of inquiries vs 88.9% for non-superhosts 
  but price nearly identically — superhost status signals operations, not premium pricing
- Bangkok's market reached a 2024 record of 148,869 reviews — 2.5× pre-COVID peak

**Clustering (K-Means, K=4)**
- 4 market segments identified: Budget Rooms (25%), Mid-Range Homes (47%), 
  High-Demand Homes (21%), Luxury Properties (7%)
- High-Demand Homes priced similarly to Mid-Range but with 3× lower 
  availability — demand pressure, not price, defines this segment

**Price Prediction**

| Model | MAE | RMSE | R² |
|-------|-----|------|----|
| Linear Regression | 958 THB | 3,536 THB | 0.450 |
| Random Forest | 719 THB | 1,925 THB | 0.617 |

- Random Forest outperforms Linear Regression by 37% on R²
- Bedrooms and neighbourhood are the strongest predictors in the RF model
- Cluster label from K-Means adds signal to both models, validating 
  the segmentation approach

---

## Pipeline
EDA (Sections 0–7) → K-Means Clustering (Section 8) → 
Price Prediction (Section 9) → Model Evaluation (Section 10)

## Tools & Libraries
Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly, GeoPandas, 
SciPy, Scikit-learn

## Data Source
[Inside Airbnb](http://insideairbnb.com) — Bangkok, Central Thailand 
(September 2025)
