# Determinants-of-second-hand-car-prices
The project sets out to identify the key specifications that influence the price of second-hand cars in German markets using BMW car dataset. I applied **multivariate regression model**, which is a powerful tool to study and quantify the relationships between the explanatory factors and the response variable.

### ⚡PROBLEM STATEMENT
What are the key factors that influence the price of BMW second-hand cars in German markets?

### ⚡ACTION
#### Step 1: Collect sample dataset
I used _a web scrapping library from Python_ to extract car listing data from _autoscout24.com_ on 22nd Jan 2021. _autoscout24.com_ has 30 million active users per month, which is a good indication of an up-to-date market data source that closely reflects the demand and supply. Moreover, the vast number of used cars listed on autoscout24 also allows a larger sample size, producing more precise estimations.

The target object is BMW cars in the German market, specifically the 3rd-generation model with 4 seats, available in popular body types: sedan, coupé, compact, and touring. After filtering out observations with less than 3 out of 9 required details, I then had a cleaned dataset of **395** pre-owned cars, each including its **price** and **8 specification details** 

#### Step 2: Specify multivariate regression model 
<p align="center"> 
<img src="https://github.com/minhanhvu/Determinants-of-second-hand-car-prices/assets/87383756/869b6a3d-20d5-4135-9611-76cc7496d128" width=60% height=60%>
</p>

#### Step 3: Check model robustness
![image](https://github.com/minhanhvu/Determinants-of-second-hand-car-prices/assets/87383756/8a3c6437-28e1-4420-8e9b-d33d8421577c)

Here I discussed the functional misspecification issues that could alter the original results. 

- White test for heteroskedasticity
- Multicollinearity test
a

### ⚡OUTCOME
The results show that car age, mileage, horsepower, and gear type have significant impacts on the variation of car prices. The cost of the BMW car decreases by 860 euros for every additional year of age. Every thousand kilometers the car run drives down its price by 76 euro. I consider these effects to be aligned with economic norms. Car age and mileage are indicators of the car's wear and tear, and signify the risk of malfunction. Therefore, customers are less willing to pay for old cars. On the other hand, the higher the horsepower, which indicates the rapidness of a car's engine, the higher the price. Besides, comparing two cars with similar profiles, an automatic BMW car is on average 2,104 euro more expensive than a BMW manual car. 

Overall, the model explains 81% of the changes in car prices, demonstrating strong explanatory power. 
### ⚡LEARNING

