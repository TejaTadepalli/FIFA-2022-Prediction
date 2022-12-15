# FIFA 2022 World Cup: Prediction

<img src="https://digitalhub.fifa.com/transform/3a170b69-b0b5-4d0c-bca0-85880a60ea1a/World-Cup-logo-landscape-on-dark?io=transform:fill&quality=75"/>

<br>

**Predicting the winner of FIFA World Cup 2022 through historical data of the matches played in previous World Cups.**

<br>

## Python Libraries Used:
- Pandas: Used for data manipulation and analysis. Also used for using dataframes for the CSV files.

- Pickle: Used for accessing the dict_table file which contains the data we have web-scrapped. This contains the fixtures of the present World Cup.

- Scipy.stats: Used for Poisson Distribution which will be later used for prediction.

#

We have used data which was web-scrapped from online available websites. We were able to get the fixture-wise data of all the matches played in the FIFA World Cup from 1930 to 2018. We have used this data to predict the winner of FIFA World Cup 2022.

We have used Poisson Distribution to predict the winner of the tournament. 
#

## Poisson Distribution
It is a discrete probability distribution that describes the number of events occuring in a fixed time interval or region of opportunity.

Poission Distribution Formula: $P(X=k) = \frac{\lambda^k e^{-\lambda}}{k!}$

Where:  
- $\lambda$ = expected number of events per time interval

- $\lambda$ = median of goals in 90 Mins (b/w 2 teams A and B)      

- x = the number of goals in a match that could be scored by Team A or B

<br>

Assumtions to be done:
1. Number of Events can be counted.
2. Occurance of events are independent.
3. The rate at which events occur is constant.
4. Two events cannot occur at the same instant in time.