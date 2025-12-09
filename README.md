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
