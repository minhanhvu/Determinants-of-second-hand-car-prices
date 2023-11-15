#### 📝 NOTE:
Here you'll find the summary of my projects. For in-depth analysis/discussion, please visit my [Gitbook](https://minh-anh-vu.gitbook.io/anh-vus-datacracy-hub/)

### ⁉️ Problem statement
The project sets out to identify the key specifications that influence the price of second-hand cars in German markets using BMW car dataset. 
### 🎬 Action
#### _Step 1_: Collect sample dataset
Used _a web scrapping library from Python_ to extract car listing data from _autoscout24.com_.

After filtering out observations with insufficient required information, I had a cleaned dataset of **395** pre-owned cars, each including its **price** and **8 specification details** 
#### _Step 2_: Collect sample dataset
Applied **multivariate regression model**, which is a powerful tool to study and quantify the relationships between the explanatory factors and the response variable.
#### _Step 3_: Check model robustness
- Discussed the functional misspecification issues that could alter the original results and suggested two alternatives.
- Conducted white test for heteroskedasticity and VIF test for multicollinearity problem and interpreted the test results

### 💡Outcome
<p align="center"> 
<img src="https://github.com/minhanhvu/Determinants-of-second-hand-car-prices/assets/87383756/b9cf703c-810d-41c8-aebe-66bae2ff6dcf" width=60% height=60%>
</p>

The results show that car age, mileage, horsepower, and gear type have significant impacts on the variation of car prices. 
- The cost of the BMW car decreases by 860 euros for every additional year of age. Every thousand kilometers the car run drives down its price by 76 euro. I consider these effects to be aligned with economic norms as car age and mileage indicate the risk of malfunction, so customers are less willing to pay for old cars. 
- On the other hand, the higher the horsepower, the higher the price. Besides, comparing two cars with similar profiles, an automatic BMW car is on average 2,104 euro more expensive than a BMW manual car. 

Overall, the model explains 81% of the changes in car prices, demonstrating strong explanatory power. 

