Project Overview:
In this project we have analysed trader transaction data and based on the analysis formulated recommendations for better trading outcomes and built one prediction and forecasting model. The data set contains transaction id, transaction size, coin, timestamp, side, size in USD, account details etc.

Objective:
Primary objective of the project is to analyse transaction data and based on the analysis recommend better trading ways to maximize gains on each transaction.
Using clustering model segregate transaction into different segments and build one prediction model to predict profit and loss based on trader behaviour and patterns in trading ways.

Dataset:
1.	Historical data
Sr. No.	Column name	Data type
1	Account	Object
2	Coin	Object
3	Execution Price	Float64
4	Size Tokens	Float64
5	Size USD	Float64
6	Side	Object
7	Timestamp IST	Object
8	Start Position	Float64
9	Direction	Object
10	Closed PnL	Float64
11	Transaction Hash	Object
12	Order ID 	Int64
13	Crossed	Bool
14	Fee	Float64
15	Trade ID	Float64
16	Timestamp	Float64

2.	Fear greed index:
Sr. No.	Column name	Data type
1	Timestamp	Int64
2	Value	Int64
3	Classification	Object
4	Date	Object



Analysis:
In analysis following analysis is carried out from historic data and fear & greed data:
1.	Average daily profit and loss of each trader.
2.	Win rate of each trader & win rate of all transactions.
3.	Win rate on each date.
4.	Average trade size of each transaction.
5.	Leverage of each transaction & distribution of leverage across accounts and dates.
6.	Number of trades per day.
7.	Long-short ratio for each account and each date & variation of long – short ratio on fear and greed days.
8.	Drawdown proxy.
9.	Variation of PnL, leverage and drawdown proxy on fear vs greed days.
10.	Win rates on fear and greed days.
11.	Trade frequency of trader on fear and greed days.
12.	Leverage of trader on fear and greed days.
13.	Long-short ratio of traders on fear and greed days.
14.	Transaction size on fear and greed days.
15.	Segmentation traders based on leverage, trade frequency and win rate.


Clustering and prediction model:

Clustering model:
Kmeans clustering model is used for clustering transactions into three segments. Segmenting transactions into different segments allows giving better recommendations to traders to maximize gains.

Prediction model:
Catboost model is used to predict PnL based on transaction data by training and fine tunning the catboost model.
SARIMAX forecasting model along with exogenous variable is used to predict future PnL by training and fine tunning SARIMAX forecasting model.

Techniques used:
1.	Python: Pandas, numpy, seaborn, matplotlib, sickit-learn, SARIMAX, Catboost etc.
2.	Table merging and group by.
3.	Aggregations.
4.	Data visualisation.
5.	Data cleaning and pre-processing.
6.	Feature engineering.
7.	Manual segmentation.
8.	Clustering.
9.	Prediction model.
10.	Time series forecasting.


Collab notebook link:
https://colab.research.google.com/drive/17MRT9Za7l34DJEr1xjb2b0eCtGByZpiJ?usp=drive_link
 

