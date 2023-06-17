# Machine Learning with R
R used to learn and visualize some economic relations in america
In this project we compared 2 ML algorithm, they are

>  <font color='red'>"Linear Regression"</font> and <font color='red'>"Random Forest"</font> 

in out dataset:
we kept the train year range between 1960 and 2005
and for test data-set, our range is: 2005 to 2020

first step:
### Collecting Dataset
here we collected several datas from different websites;
for:
<br>GDP:
<br>https://data.worldbank.org/indicator/NY.GDP.PCAP.CD?end=2021&locations=US&start=1960&view=chart
<br>Inflation: 
<br>https://ycharts.com/indicators/us_inflation_rate#:~:text=Basic%20Info,in%20price%20over%20a%20year
<br>Interest Rate: 
<br>https://tradingeconomics.com/united-states/interest-rate#:~:text=Interest%20Rate%20in%20the%20United,percent%20in%20December%20of%202008
<br>Oil Price: 
<br>https://www.statista.com/statistics/262860/uk-brent-crude-oil-price-changes-since-1976/
<br>Per Capita Income: 
<br>https://data.worldbank.org/indicator/NY.GDP.PCAP.CD?end=2021&locations=US&start=1960&view=chart
<br>Population: 
<br>https://www.macrotrends.net/countries/USA/united-states/population
<br>sP 500: 
<br>https://www.macrotrends.net/2324/sp-500-historical-chart-data
<br>Unemployment Rate: 
<br>https://www.thebalancemoney.com/unemployment-rate-by-year-3305506

### Correlation Matrix
In this chart, we showed the relationships of the data columns with each other in the form of a matrix.
 
![alt text]([http://url/to/img.png](https://github.com/TkRsln/MLwithR_1/blob/main/pictures/CorMatrix.png?raw=true))

### 1st Predict Model: Inflation - Unemployment
We tried to predict inflation based on the unemployment rate.
According to this prediction, Random forest gave better results by MSE value.
Random Forest MSE 10.26008
Linear Regression MSE 11.12079

Here is the chart:
![alt text](https://github.com/TkRsln/MLwithR_1/blob/main/pictures/unemp_inf_predict.png?raw=true)


### 2nd Predict Model: Inflation - Interest Rate
We tried to predict inflation based on the Interest Rate rate.
According to this prediction, Random forest gave better results by MSE value.
Linear Regression MSE: 2.077702
RandomForest MSE: 1.505035

Here is the chart:
![alt text](https://github.com/TkRsln/MLwithR_1/blob/main/pictures/unemp_inf_predict.png?raw=true)

### 3rd Predict Model: Inflation_Rate  with Unemployment_Rate + S_P_500 + Oil._Price + Interest_Rates 
We tried to predict inflation based on the Unemployment_Rate, S_P_500, Oil._Price and Interest_Rates 
According to this prediction, Linear Regression gave better results by MSE value.
Linear Regression MSE: 2.871658
RF MSE 6.122257

Here is the chart:
![alt text]([http://url/to/img.png](https://github.com/TkRsln/MLwithR_1/blob/main/pictures/4_inf_predict.png?raw=true))


## Sum
From the graph shown below, you can see how much "MSE" value the Learning methods produce in which models.

![alt text](https://github.com/TkRsln/MLwithR_1/blob/main/pictures/ConfusionMatrix.png?raw=true)

Considering these 3 learning conditions, the average "MSE" values of the learning methods are:
Random Forest avg. MSE: 5.962457
Linear Regression avg. MSE: 5.356715



