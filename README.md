# Determinants-of-second-hand-car-prices
The project identifies the key specifications influencing the price of second-hand cars in German markets, using BMW car dataset.
### ⚡PROBLEM STATEMENT
What are the key factors that influence the price of second-hand cars in German markets?
### ⚡ACTION
#### Step 1: Collect sample dataset
I used _a web scrapping library from Python_ to extract car listing data from _autoscout24.com_ on 22nd Jan 2021. I chose autoscout24.com for its significant number of active users, which is a good indication of an up-to-date market data source that closely reflects the demand and supply. Moreover, the vast number of used cars listed on autoscout24 also allows a larger sample size, producing more precise estimations.

I focus on BMW cars in the German market, specifically the 3rd-generation model with 4 seats, available in popular body types: sedan, coupé, compact, and touring. After filtering out observations with less than 3 out of 9 required details, I then had a cleaned dataset of **395** pre-owned cars, each including its **price** and **8 specification details.**

#### Step 2: Specify multivariate regression model 

<p align="center"> 
<img src="https://github.com/minhanhvu/Determinants-of-second-hand-car-prices/assets/87383756/8da1c95b-0085-4b38-8261-5750d8b3e8da" width=60% height=60%>
</p>
<p align="center"> Correlation matrix between dependent variables
</p>
<p align="center"> 
<img src="https://github.com/minhanhvu/Determinants-of-second-hand-car-prices/assets/87383756/869b6a3d-20d5-4135-9611-76cc7496d128" width=60% height=60%>
</p>

**Dependent variable:** Car price

**Independent variables:**
1. Mileage (number of kilometers driven)
2. Year of first registration
3. Horsepower
4. Number of previous owners
5. Gear type (automatic/manual)
6. Fuel type (gasoline/diesel)
7. Fuel consumption per 100km
8. CO2 emission per km

#### Step 3: Check model robustness 

### ⚡OUTCOME

### ⚡LEARNING
