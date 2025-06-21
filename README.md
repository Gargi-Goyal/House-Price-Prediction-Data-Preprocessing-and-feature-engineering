# House Price Prediction Assignment

## Description
A data preprocessing and feature engineering project for the [Kaggle House Prices dataset](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data).

## Files
- `house_price_prediction.ipynb`: Jupyter notebook with preprocessing code
- `data/`: Folder for dataset (create this manually)
  - Download `train.csv` and `test.csv` from Kaggle and place here

## How to Run
1. Download the dataset from Kaggle (link above)
2. Create a `data` folder in the project directory
3. Place `train.csv` and `test.csv` in the `data` folder
4. Open and run the Jupyter notebook

## Preprocessing Steps
1. **Handled Missing Values**:
   - Filled categorical missing values with `'None'`
   - Filled numerical missing values with `0`

2. **Feature Engineering**:
   - Created:
     - `TotalSF`: Total living area (1stFlr + 2ndFlr + Basement)
     - `TotalBath`: Weighted sum of bathrooms
     - `TotalPorch`: Combined porch area
   - Encoded categorical variables (ordinal + one-hot encoding)

3. **Data Transformation**:
   - Applied log transformation to `SalePrice` for normality

