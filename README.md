# House Price Prediction Assignment

## Description
A data preprocessing and feature engineering project for the [Kaggle House Prices dataset](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data).

## File
- `house_price_prediction.ipynb`: Jupyter notebook with preprocessing code

## How to Run
1. Download the dataset from Kaggle (link above)
2. Open the .ipynb file 
3. Paste the path of train and test.csv path in the code(of.ipynb file)
4. run the Jupyter notebook

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

## Requirements
- Python 3.x
- Jupyter Notebook
- Libraries: pandas, numpy, matplotlib, seaborn

Install with:
```bash
pip install pandas numpy matplotlib seaborn jupyter
