# Logistic Regression and Model Selection

A binary classification study using the breast cancer dataset included in scikit-learn. The notebook builds the classifier and evaluates feature transformations with a held-out validation split.

## What it covers

- Binary cross-entropy from logits and gradient checks
- Standardization fitted on training data only
- PCA and quadratic feature expansion
- Validation-based comparison using ROC-AUC and classification metrics
- Final evaluation on a separate test split

## Run locally

Python 3.10 or newer is recommended. Create an environment and install the dependencies:

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
python -m pip install -r requirements.txt
jupyter lab
```

Open `logistic_regression.ipynb` and run all cells. The dataset is fetched through scikit-learn; no local dataset files are needed.

## Validation

The recorded run selected the standardized-feature pipeline using validation ROC-AUC (0.9836). Its test ROC-AUC was 0.9987. The test split is used only for the final evaluation.

## Attribution

This is an adapted solution to an educational laboratory. The original assignment and its course attribution are preserved in the notebook.
