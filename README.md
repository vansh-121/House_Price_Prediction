# House Price Prediction (Linear Regression)

A simple, end-to-end notebook that trains a linear regression model to predict house prices. It loads a CSV dataset from Google Drive, performs a train/test split, standardizes features, fits a `LinearRegression` model, and evaluates with $R^2$.

## Project Structure

- `House_Price_Prediction_(Linear_Regression).ipynb` - main notebook

## Dataset

The notebook downloads the dataset directly from Google Drive:

- https://drive.google.com/uc?export=download&id=1fx9qqGQqEQxpOizGodP3RTIZFsNeFw2L

The target column is `House_Price`. All other columns are treated as features.

## Requirements

- Python 3.8+
- pandas
- scikit-learn

You can install the dependencies with:

```bash
pip install pandas scikit-learn
```

## How to Run

1. Open the notebook `House_Price_Prediction_(Linear_Regression).ipynb` in Jupyter or VS Code.
2. Run cells from top to bottom.

The notebook will:

- Load the dataset
- Split into train/test sets
- Standardize features
- Train a linear regression model
- Make predictions and report $R^2$

## Notes

- Standardization is fitted on the training set and applied to the test set.
- The model performance is reported with `lr.score(X_test, Y_test)`.

## License

If you plan to share or reuse this project, add a license of your choice.
