

# Cash-Flow-Forecasting
Challenge in collaboration with LUISS and one of Italy's most important energy companies


## Affinity Analysis (Market Basket Analysis)
Market Basket Analysis (MBA) is an accidental transaction pattern that purchasing some products will affect the purchasing of other products. MBA is used to predict what products that customer interested in. It’s a kind of knowledge discovery in data (KDD) and this technique can be applied in various fields of work.
Before performing the affinity analysis, it is strongly advised to handle with missing values, either drop them, or replace them according to a predefined methodology. We decided to drop them because some of them are variables for identification purpose. In our understanding of the datasets provided, we decided to consider only positive values of column Amount, because in EDA, we found out that most of the Amount were positive, which intuitively we associate them as cost/liability since our main goal is to estimate cash flows related to the account payable in the 1st and 2nd quarters of 2022.

![immagine](https://user-images.githubusercontent.com/93279084/168492496-d52310b0-91e7-45d6-b1a1-8f11a11a62fe.png)



## Time Series Forecasting 

### Prophet
The first algorithm is Prophet. It is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.


### LSTM
Long Short-Term Memory (LSTM). LSTM is a Recurrent neural network that learn to predict the future from sequences of varying lengths use LSTM 
cells. Recurrent neural networks, unlike ARIMA and Prophet, can deal with any type of sequential data and are not limited to time series. The fundamental goal of LSTM 
cells is to remember the critical bits of the sequence while forgetting the less significant ones. This is accomplished using so-called gates, which are functions with 
various learning objectives.



![immagine](https://user-images.githubusercontent.com/93279084/168492587-6280e555-dde2-4be0-a5b6-64fe9b385613.png)






In conclusion, through R2, MSE and RMSE we evaluated the models and chose the one that, in our view, is most accurate in calculating cash flow . 


## Authors 
- Enrico Romano
- Simone Lu
- Leonardo Crescenzi



