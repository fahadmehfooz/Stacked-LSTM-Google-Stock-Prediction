# Stacked-LSTM-Google-Stock-Prediction

* We are provided with 6 variables describing the stock market trend for google. 
* The task is to predict the future stock market price on the basis of past data.
* Here, I have taken past 100 days data to predict the next day's stock price.
* I used an LSTM model because of it is powerful in storing sequence.
* After building the model, I used keras tuner to tune the hyperparameters of the model.

## Resources and Tools Used
**Tools:** Jupyter Notebook

**Packages:** Pandas, NumPy, sklearn, Matplotlib, seaborn, kerastuner.
## Data Used
About the data: The art of forecasting stock prices has been a difficult task for many of the researchers and analysts. In fact, investors are highly interested in the research area of stock price prediction. For a good and successful investment, many investors are keen on knowing the future situation of the stock market. Good and effective prediction systems for the stock market help traders, investors, and analyst by providing supportive information like the future direction of the stock market. In this work, we present a recurrent neural network (RNN) and Long Short-Term Memory (LSTM) approach to predict stock market indices.

**Data Source**: https://www.kaggle.com/fahadmehfoooz/stacked-lstm-google-stock-prediction/data

## Data Wrangling And Visualizations

* Scaling data using a MinMaxScaler.
* Preparing train and test data.
* Taking data for past 100 days for next prediction.
* Plotting loss, and validation loss.

![alt text](https://raw.githubusercontent.com/fahadmehfooz/Stacked-LSTM-Google-Stock-Prediction/main/images/__results___19_0.png)


## Model Building 

* I took a split on the data with training data as 65% and test data as 35%. 
* Built base level model using an LSTM stacked with multiple layers.
* To avoid overfitting, I have used dropout layers.
* Compiled the model using adam optimizer and mean_squared_error loss.
* After building base model, I tuned the hyperparameters using keras tuner search with 5 trials.

## Loss Used For Evaluation
* RMSE

## Model performance

**Results:**

* Train RMSE:  772.060016780815
* Test RMSE:  734.1198356359321
