# Stock Price Prediction 
## Introduction
Stock market prediction is the act of trying to determine the future value of a company stock
or other financial instrument traded on an exchange. Here the prediction is the next day's closing price of cmb China with the stock code 600036.SH.

## Libraries
* Numpy
* Pandas
* Scikit Learn
* Keras
* Matplotlib

## File Description
* <strong>Data Folder</strong>  
  It contains the historical data of cmb China stock.
  
* <strong>Model Folder</strong>  
  It contains the saved keras models in .h5 and .json format
  
* <strong>Result Folder</strong>  
  It contains all the plots, Score, and Prediction value in excel format
  
* <strong>Utils Folder</strong>  
  It contains all utility python scripts for plotting, training model, saving and loading models and creating input data
  
* **Investment_and_Trading_LSTM.ipynb**
  
  The main script file to realize the project, including data fetching, data preprocessing, data loading and predictions: 
  
  	- single feature as opening price to predict the next day's closing price
  	- finding best pair of hyperparameters model that could help in refining the model
  	- finding the best selecting of features for predicting the next day's closing price
  	- At last, after getting the most optimized model, predicting the next day's closing price and get final result
- **DSND_capstone_project_investment and trading.pdf**  
  The capstone report.

## Results

Initially, the r2 score on testing data was 0.793 and mse score was 2.799 for predicting the next day's closing price.  

<img src='https://github.com/zxhx/DSND_capstone_project_investment-and-trading/blob/master/result/single_attribute/output_test.png' width=400px>

After hypermeter optimization the r2 score increased to 0.89 and mse value decreased to 1.45.  

<img src='https://github.com/zxhx/DSND_capstone_project_investment-and-trading/blob/master/result/hyperParaModels/output.png' width=400px>

Then, we applied feature importance after that the r2 score increased to 0.91 and mse value decreased to 1.09.

<img src='https://github.com/zxhx/DSND_capstone_project_investment-and-trading/blob/master/result/final_model/output_test.png' width=400px>

  