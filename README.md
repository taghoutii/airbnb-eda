# Bangkok Airbnb EDA
# Bangkok Airbnb EDA
### What Makes a Successful Airbnb Listing in Bangkok?

Exploratory Data Analysis on 23,000+ Bangkok Airbnb listings using data from 
[Inside Airbnb](http://insideairbnb.com) (September 2025).

---

## Key Findings

**Price Drivers**
Accommodation size is the dominant price driver — each additional guest capacity 
increases nightly price by ~19%. Review scores have near-zero correlation with price.

**Neighbourhood Patterns**
Bangkok follows a centre-periphery pricing structure. Parthum Wan (2,248 THB/night) 
commands 4× the price of peripheral areas. High listing volume does not equal high 
price — location prestige matters more than listing density.

**Host Performance**
Superhost status signals operational excellence, not premium pricing. Superhosts 
maintain 99.1% response rate and 93.3% acceptance rate vs 88.9% and 78.6% for 
non-superhosts — yet price nearly identically.

**Market Recovery**
Bangkok's Airbnb market has fully recovered from COVID-19, reaching a 2024 record 
of 148,869 reviews — 2.5× the pre-COVID peak.

---

## Project Structure
```
airbnb-eda/
├── data/                    # Raw data files (not tracked by Git)
│   ├── listings.csv.gz
│   ├── calendar.csv.gz
│   ├── reviews.csv.gz
│   └── neighbourhoods.geojson
├── notebooks/
│   └── 01_eda.ipynb         # Main analysis notebook
├── .gitignore
├── requirements.txt
└── README.md
```

## Tools & Libraries
Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly, GeoPandas, SciPy

## Data Source
[Inside Airbnb](http://insideairbnb.com) — Bangkok, Central Thailand (September 2025)

## Author
Eya 