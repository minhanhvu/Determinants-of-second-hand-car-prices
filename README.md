# Determinants-of-second-hand-car-prices
The project sets out to identify the key specifications that influence the price of second-hand cars in German markets using BMW car dataset. I applied the **multivariate regression model**, which is a powerful tool to study and quantify the relationships between the explanatory factors and the response variable (car prices in this project). 

### ⚡PROBLEM STATEMENT
What are the key factors that influence the price of BMW second-hand cars in German markets?

### ⚡ACTION
#### Step 1: Collect sample dataset
I used _a web scrapping library from Python_ to extract car listing data from _autoscout24.com_ on 22nd Jan 2021. _autoscout24.com_ has a significant number of active users, which is a good indication of an up-to-date market data source that closely reflects the demand and supply. Moreover, the vast number of used cars listed on autoscout24 also allows a larger sample size, producing more precise estimations.

The target object is BMW cars in the German market, specifically the 3rd-generation model with 4 seats, available in popular body types: sedan, coupé, compact, and touring. After filtering out observations with less than 3 out of 9 required details, I then had a cleaned dataset of **395** pre-owned cars, each including its **price** and **8 specification details** 

#### Step 2: Specify multivariate regression model 
Correlation matrix
Heteroskedasticity and multicollinearity

<p align="center"> 
<img src="https://github.com/minhanhvu/Determinants-of-second-hand-car-prices/assets/87383756/869b6a3d-20d5-4135-9611-76cc7496d128" width=60% height=60%>
</p>

#### Step 3: Check model robustness 
Discussion focuses on the endogeneity and functional misspecification problems

### ⚡OUTCOME
The results show that car age, mileage, horsepower, and gear type have significant impacts on the variation of car prices. The older the car and the longer it has been driven, the cheaper it is. On the other hand, the higher the horsepower, which indicates the rapidness of a car's engine, the higher the price. Besides, comparing two cars with similar profiles, an automatic BMW car is on average 2,104 euro more expensive than a BMW manual car. Overall, the model explains 81% of the changes in car prices, demonstrating strong explanatory power. 
### ⚡LEARNING

