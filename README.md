# Titanic Survival Prediction

Compact Kaggle-style starter that trains a logistic regression model on the Titanic dataset using scikit-learn. Feature engineering is prototyped in `notebooks/main.ipynb`, and predictions for the competition test split are exported as `result.csv`.

## Repository layout

- `data/`: Original Kaggle CSVs (`train.csv`, `test.csv`, `gender_submission.csv`).
- `notebooks/main.ipynb`: End-to-end preprocessing, model fitting, and CSV export logic.
- `submissions/`: Keep generated submissions here (ignored by Git).

## Quick start

```bash
python -m venv .venv
.venv\Scripts\activate          # Windows
pip install -U pip pandas numpy matplotlib scikit-learn
jupyter notebook notebooks/main.ipynb
```

1. Execute the notebook top-to-bottom (adjust feature engineering as desired).
2. The final cell writes `result.csv`, ready for Kaggle upload.

## Next steps

- Improve feature coverage (e.g., age imputation, family size, fare bands).
- Log experiments and scores to compare iterations quickly.
