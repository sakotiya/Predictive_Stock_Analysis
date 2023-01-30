# Finance_Group_Project

## Intro 
In this project our goal is to use multiple indices to show correlations between sectors and Bitcoin. We will be analyzing Stocks in two manners, internal and external correlation. Internal correlation will be between different sectors and will determine if there is a correlation between high & low prices and volume trading in a span of 10 years.  External correlation will be between all sectors and Bitcoin. 

Our steps for this project include attaining ten years of stock data for five sectors that include HealthCare, Technology, Automobile, Materials, Commerce, and Bitcoin. Data for the former sectors was obtained from Yahoo Finance in the form of CSV files. Yahoo finance provides CSV files with the date; open, high, low, close, adj_close, and volume.
Databases for these sectors were created via Python and SQL and output as CSV files. These databases were normalized using in MinMaxScaler from sklearn.preprocessing.

![image](https://user-images.githubusercontent.com/111551902/215545453-294fd740-6eb2-49e7-91cd-9242850460ad.png)


## Healthcare 
Tickers utilized to represent the healthcare sector were selected based off of market cap from yahoo finance. 

AbbVie, Inc

AMN Healthcare Services, Inc

Diversified Healthcare Trust

Gilead Science, Inc

GSK plc

HCA Healthcare

Johnson and Johnson

Omega Healthcare Investors

Sanofi

Takeda Pharmaceutical Company


Using yahoo finance, historical ticker data for each stock was pulled from January 2013 to January 2023. Yahoo finance provides CSV files with date of information; open, high, low, close, adj_close, and volume. For this project we are only interested in volume, high, and low data. Thus, SQL was used to pull and merge data from individual csv files.

### Analysis
However, as we are trying to merge multiple data sets across different sectors, it was found that the data needs to be normalized. In this case, MinMaxScaler from sklearn.preprocessing was used to normalize volume, high, and low to a set of data point between 0 and 1. This allows us to compare our large sets of data more accurately. 


#### Example of SQL code
![image](https://user-images.githubusercontent.com/111551902/215550526-b165cd11-5f66-4d3e-bdb6-b6219f3e86ea.png)



![image](https://user-images.githubusercontent.com/111551902/215550673-7c94624a-c978-4459-9b41-eb230d3ffcb5.png)


![image](https://user-images.githubusercontent.com/111551902/215550777-90f6b81f-9d7a-4148-b217-92432f40196c.png)



##### Example of Scaler Python Code
![image](https://user-images.githubusercontent.com/111551902/215550861-6cc1a42d-ac4f-4481-a7e0-7d22ac7d2240.png)

