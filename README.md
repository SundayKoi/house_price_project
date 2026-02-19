# USA Real Estate Market Analysis & Price Prediction

An end-to-end data science project analyzing 2.2 million US real estate listings to uncover market trends and predict house prices using machine learning.

## Results
| Metric | Score |
|---|---|
| R2 Score | 0.859 |
| Mean Absolute Error | $66,446 |

## Project Structure
```
├── usa_real_estate_analysis.ipynb  # Main notebook
├── avg_price_by_state.html         # Interactive state map
├── avg_price_by_zip.html           # Interactive zip code map
└── README.md
```

## Key Findings
- **Location is everything** — zip code accounts for 53% of feature importance, confirming the "location, location, location" rule
- **California** is the most expensive state at ~$1M average
- **House size** is the second most important predictor at 19%
- Model achieves **R2 of 0.859** — explaining 85.9% of price variation

## Features Used
- Bedrooms, Bathrooms
- House size (sq ft), Lot size (acres)
- Zip code, City, State

## Tech Stack
- **Data Processing:** pandas, numpy
- **Machine Learning:** scikit-learn (Random Forest), XGBoost
- **Visualization:** matplotlib, seaborn, folium, pgeocode
- **Optimization:** GridSearchCV with 3-fold cross validation

## Setup
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost folium pgeocode kagglehub
```

Download the dataset from [Kaggle](https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset) and place `realtor-data.zip.csv` in the project directory.

## Interactive Maps
The project generates two interactive HTML maps:
- **State level** — click any state to see avg, median, min, max prices
- **Zip code level** — bubble size represents average price, click for details
