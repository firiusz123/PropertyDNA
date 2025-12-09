PropertyDNA

PropertyDNA — Analysis of property listings to predict building year from rental/buying data in Poland.

Overview

This project analyses a dataset of rental and sale listings for flats and houses in Poland. Using machine‑learning / data‑analysis techniques, it shows that it’s possible to predict the building year of a given listing with a mean error of ≈ ±7.4 years — which could be useful for researchers, real‑estate analytics, or data‑driven property valuation studies.

Key Features

- A processed dataset of property listings (renting / buying) with relevant features (e.g. location, price, size, amenities, etc.).
- Data analysis and preprocessing (cleaning, feature extraction, feature engineering).
- A prediction model (or multiple models) to estimate building year based on listing metadata.
- Jupyter‑notebook with end-to-end analysis: data cleaning → training → evaluation → results.
- Evaluation showing the predictive error (~7.4 years), plus relevant statistics / visualisations.

Repository Structure

/          — root
Project&Lab_ipynb_.ipynb   — main analysis notebook (data exploration, preprocessing, modeling, evaluation)
/data/ (if present)          — raw or processed datasets (CSV/JSON/etc)
README.md                    — this readme

Requirements & Setup

- Python 3.x
- Typical data‑science stack (e.g. pandas, NumPy, scikit-learn, possibly matplotlib / seaborn)
- Jupyter (for working with the provided notebook)

Example setup:

git clone https://github.com/firiusz123/PropertyDNA.git
cd PropertyDNA
python -m venv venv
source venv/bin/activate         # or `venv\Scripts\activate` on Windows
pip install -r requirements.txt  # if you provide it
jupyter notebook Project&Lab_ipynb_.ipynb

Usage / Quick Start

1. Load the notebook Project&Lab_ipynb_.ipynb.
2. Run cells in order: data loading → cleaning/preprocessing → feature engineering → model training → evaluation.
3. Inspect results: predicted building years, error metrics, maybe plots.
4. (Optional) You can extend the analysis: try different feature sets, other models (e.g. regression, ensemble methods), cross‑validation, or further data enrichment.

Results & Interpretation

- The model achieves a mean error around ±7.4 years on predicting building year.
- This demonstrates that listing metadata (price, area, number of rooms, amenities, etc.) carries some signal about building age — but predictions remain approximate.
- Use cases: rough estimation of building year when explicit data is missing; statistical analysis across many listings; data-driven real-estate market studies.

Potential Improvements / Roadmap

- Expand the dataset (more listings, more regions) — more data usually improves model robustness.
- Feature engineering: include neighbourhood data, building type, amenities, or external socio‑economic factors.
- Use more advanced models (e.g. gradient boosting, neural networks) and evaluate their performance.
- Cross‑validation, model hyperparameter tuning, error analysis.
- Provide a cleaned dataset and a versioned data‑processing pipeline (so others can reproduce results).
- Add documentation (requirements, data schema, usage examples).

Contribution

Contributions are welcome! If you want to help — e.g.:

- Add more data, extend dataset to other regions.
- Improve preprocessing / feature engineering.
- Experiment with other models or evaluation metrics.
- Document usage / create scripts (notebooks → scripts) for easier reuse.

Please create an issue or a pull request to propose changes.

License

Specify your preferred license (e.g. MIT, GPL‑3.0, etc.). If not decided yet, choose a permissive open‑source license to allow reuse.

Date: 2025-12-09
