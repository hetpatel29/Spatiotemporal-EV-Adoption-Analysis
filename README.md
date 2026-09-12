# Spatiotemporal EV Adoption Analysis

Exploratory and predictive analysis of electric vehicle registrations in Washington State. The notebook examines adoption over time, geographic concentration, vehicle range, manufacturer and model composition, and classification of battery electric vehicles (BEVs) versus plug-in hybrid electric vehicles (PHEVs).

## Project Files

- `ev_adoption_analysis.ipynb` - analysis notebook with tables, visualizations, statistical tests, and machine-learning models.
- `Electric_Vehicle_Population_Data.csv` - vehicle registration dataset used by the notebook.

## Requirements

- Python 3.10 or newer
- Jupyter Notebook or VS Code with the Jupyter extension

Install the Python dependencies with:

```bash
python -m pip install numpy pandas matplotlib scipy scikit-learn jupyter
```

## Run the Analysis

1. Clone the repository.
2. Open `ev_adoption_analysis.ipynb` in Jupyter or VS Code.
3. Select a Python kernel with the required dependencies.
4. Run all cells from top to bottom.

The notebook automatically loads `Electric_Vehicle_Population_Data.csv` from the project directory.

## Analysis Coverage

- Dataset quality and missing-value summaries
- BEV and PHEV distribution through model year 2024
- Leading manufacturers, models, counties, and cities
- Spatial registration density using vehicle coordinates
- Reported electric-range distributions and trends
- Correlation and ANOVA tests
- County/type chi-square analysis with Cramer's V
- Logistic regression, decision tree, and random forest classification
- Original versus balanced training comparisons using accuracy, PHEV recall, F1, ROC-AUC, and confusion matrices

## Reproducibility Notes

The notebook uses a fixed random state of `42` for reproducible model comparisons. The final reporting cell can disable full model retraining with `RUN_FULL_MODELING`; set it to `True` when regenerating the complete modeling outputs is required.