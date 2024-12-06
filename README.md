# Final Report
## Abstract:

## Introduction and Data Description:
In this project, we will design an algorithm to most efficiently predict which team in the National Basketball Association (NBA) will be the best. We will also design an algorithm to predict if a player is an all-star for a specific season. To determine what teams are best we will use specific team data that historically correlates to championships. Specifically, we will use data like ORTG (Offensive Rating), where the higher the rating, the better the team's offense, DRTG (Defensive Rating), where the lower the rating, the better the team’s defense, and TO%, the percentage of possesions that end in turnovers for a team . For determining what player is an all-star, we will use their total points, total rebounds, along with the amount of games they played in a season.
## Method:


## Results:

### Fig 1 (Model 1):
<img width="687" alt="Screenshot 2024-12-06 at 3 49 57 PM" src="https://github.com/user-attachments/assets/8a75320f-f6f4-4aaa-a8e2-b2f5ddccab93">

As can be seen in the above figure, the histogram roughly follows a symmetrical, normal distribution, ideal for a regression model. Due to the majority of the residuals being close to 0, this indicates that our models predictions were quite close to the actual values for most of the data, although at times the observed value was slighly larger than the predicted value.

### Fig 2 (Model 1):
<img width="629" alt="Screenshot 2024-12-06 at 4 13 16 PM" src="https://github.com/user-attachments/assets/e4606a74-fb37-4b99-9f65-296f65931ce7">

As can be seen in the above figure, there are no clear outliers in the residuals, and they generally cluster closer to 0. Along with this, we see no uniform pattern in the plot of residuals, a good sign for our model. 

## Discussion:
For our first model, we clearly saw that picking ORTG, DRTG, and TO% of a team were very strong indicators of how good a team was. For example, our ML model correctly predicted the 2024 Boston Celtics, who won the championship, to be the best team, and predicted the 2016 Philadelphia 76ers (who had a record of 10 wins to 72 losses) to be the worst team. Furthermore, our ML model generated an R^2 of 0.8958476288965742, showing that our ML model is quite accurate in predicting the actual data.Our ML model also generated an MSE of 14.706814990817946, which shows that there is a low variance in errors in our ML model. Although our model is quite accurate, it is not perfect. Thus, you could take it's predictions at face value, but they might not always be correct. Due to this, we might want to see if any other team analytics correlate more to the success of a team, and add that analytic to our model to make it more accurate. 
