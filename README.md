# ARKK ETF Price Prediction

This project applies deep learning techniques to predict the adjusted closing price of the ARKK ETF using historical stock market data.  
The goal is to build and compare models to accurately forecast the next day's price.

## Dataset

The dataset used is `ARKK.csv`, containing daily stock data with features such as Open, High, Low, Close, Adjusted Close, and Volume.  
It has 1363 daily records spanning multiple years.

## Tools Used

- Python (Jupyter Notebook)  
- pandas, numpy  
- matplotlib  
- scikit-learn  
- TensorFlow (Keras)

## Models Trained

Three models were trained and compared:

- **Baseline Model**: Predicts the next price as the last observed price.  
- **Initial LSTM Model**: Univariate LSTM using only Adjusted Close price.  
- **Optimized LSTM Model**: Improved LSTM with hyperparameter tuning.

## Results Summary

| Model           | MAE    | RMSE   |
|-----------------|--------|--------|
| Baseline        | 0.7390 | 1.1290 |
| Initial LSTM    | 1.4647 | 2.0757 |
| Optimized LSTM  | 0.9501 | 1.4301 |

The optimized LSTM model showed significant improvement over the initial LSTM but did not fully surpass the baseline.

## Conclusion

This project demonstrates the application of LSTM networks to time series forecasting of stock prices.  
While the baseline model performed strongly due to market price stability, the optimized LSTM was able to capture underlying trends and reduce prediction errors significantly compared to the initial model.  
The analysis illustrates the importance of model evaluation, tuning, and realistic expectations in financial forecasting.

## Files

- `ARKK_ETF.ipynb`: Full analysis and modeling notebook.  
- `ARKK.csv`: Dataset file (add or link as appropriate).

## Dataset Source

The dataset was obtained from Kaggle Stock Market datasets.

## How to Use

1. Clone this repository:

```
git clone https://github.com/yourusername/arkk-etf-price-prediction.git
```


2. Open the notebook:

- Use Jupyter Notebook or Jupyter Lab.  
- Run the cells sequentially.

3. Requirements:

- pandas  
- numpy  
- matplotlib  
- scikit-learn  
- tensorflow  
