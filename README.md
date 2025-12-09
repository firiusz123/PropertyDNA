# PropertyDNA

**PropertyDNA** — Analysis of property listings to predict building year from rental/buying data in Poland.

## Overview

This project analyses a dataset of rental and sale listings for flats and houses in Poland. Using machine-learning and data-analysis techniques, it is possible to predict the building year of a given listing with a mean error of ≈ ±7.4 years. This can be useful for researchers, real-estate analytics, or data-driven property valuation studies.

## Key Features

- Processed dataset of property listings (renting/buying) with relevant features (e.g., location, price, size, amenities, etc.).
- Data analysis and preprocessing (cleaning, feature extraction, feature engineering).
- Prediction model(s) to estimate building year based on listing metadata.
- Jupyter notebook with end-to-end analysis: data cleaning → training → evaluation → results.
- Evaluation showing predictive error (~7.4 years), plus relevant statistics and visualizations.

## Requirements & Setup

- Python 3.x
- Data science libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`/`seaborn` (for plotting)
- Jupyter Notebook

### Example setup

```bash
git clone https://github.com/firiusz123/PropertyDNA.git
cd PropertyDNA
python -m venv venv
source venv/bin/activate         # or `venv\Scripts\activate` on Windows
pip install -r requirements.txt  # if provided
jupyter notebook Project&Lab_ipynb_.ipynb
```
## Model Peak Performance

The following results come from the best-performing model after full hyperparameter optimization (80 fits total across 4-fold CV):
Fitting 4 folds for each of 20 candidates, totalling 80 fits

Best parameters:
- **colsample_bytree:** 0.7989499894055425  
- **gamma:** 4.609371175115584  
- **learning_rate:** 0.03654775061557585  
- **max_depth:** 25  
- **min_child_weight:** 9  
- **n_estimators:** 495  
- **subsample:** 0.9222669243390758

MAE: 7.4014 Years
RMSE: 13.1610 Years
STD of prediction errors: 13.1598 Years



