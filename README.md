# House Price Prediction (Using Regression)

A comprehensive notebook for predicting house prices using multiple regression models. The project loads a dataset from Google Drive, performs feature engineering, and compares Linear Regression, Ridge Regression, and Lasso Regression models.

## Project Structure

- `House_Price_Prediction.ipynb` - main notebook

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

1. Open the notebook `House_Price_Prediction.ipynb` in Jupyter or VS Code.
2. Run cells from top to bottom.

## Notebook Overview

### Data Loading & Preparation
- Load dataset from Google Drive using pandas
- Separate features (X) and target variable (Y)
- Split data into train/test sets (80/20 split, random_state=51)

### Feature Scaling
- Apply StandardScaler to normalize features
- Fit on training set and apply to test set

### Model Training & Evaluation
The notebook trains and evaluates three regression models:

1. **Linear Regression** - Baseline model using `LinearRegression()`
2. **Ridge Regression** - L2 regularized linear regression using `Ridge()`
3. **Lasso Regression** - L1 regularized linear regression using `Lasso(alpha=3)`

Each model is evaluated using the $R^2$ score on the test set.

## Notes

- Standardization is fitted on the training set and applied to the test set to prevent data leakage.
- The model performance is reported using `score()` method which computes $R^2$.
- Ridge and Lasso regression help prevent overfitting through different regularization techniques.

## License

If you plan to share or reuse this project, add a license of your choice.
