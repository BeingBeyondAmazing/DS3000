# Final Report
## Abstract:

## Introduction and Data Description:
In this project, we will design an algorithm to most efficiently predict which team in the National Basketball Association (NBA) will be the best. We will also design an algorithm to predict if a player is an all-star for a specific season. To determine what teams are best we will use specific team data that historically correlates to championships. Specifically, we will use data like ORTG (Offensive Rating), where the higher the rating, the better the team's offense, DRTG (Defensive Rating), where the lower the rating, the better the team’s defense, and TO%, the percentage of possesions that end in turnovers for a team . For determining what player is an all-star, we will use their average points, rebounds, and assists per game, along with the amount of games they played in a season.
## Method:


## Results:

### Fig 1 (Model 1):
<img width="687" alt="Screenshot 2024-12-06 at 3 49 57 PM" src="https://github.com/user-attachments/assets/8a75320f-f6f4-4aaa-a8e2-b2f5ddccab93">

As can be seen in the above figure, the histogram roughly follows a symmetrical, normal distribution, ideal for a regression model. Due to the majority of the residuals being close to 0, this indicates that our models predictions were quite close to the actual values for most of the data, although at times the observed value was slighly larger than the predicted value.

### Fig 2 (Model 1):
<img width="629" alt="Screenshot 2024-12-06 at 4 13 16 PM" src="https://github.com/user-attachments/assets/e4606a74-fb37-4b99-9f65-296f65931ce7">

As can be seen in the above figure, there are no clear outliers in the residuals, and they generally cluster closer to 0. Along with this, we see no uniform pattern in the plot of residuals, a good sign for our model. 

## Discussion:
For our first model, we clearly saw that picking ORTG, DRTG, and TO% of a team were very strong indicators of how good a team was. We were able to see this, as our model quite accurately predicted how good a team would be with the data we selected.
