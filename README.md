# Final Report
## Abstract:
In this project, we used NBA player and team data to answer two questions: can we use team stats to predict the amount of wins a team will get and can we use player stars to classify all star and non all star players? To answer the first question, we used a multiple linear regression model taking in Offensive rating, Devensive rating, and turnover percentage to predict total wins. This model proved to be very effective, predicting with a high r^2 and low MSE. We answered the second question with a random forest classification model taking in player points, total rebounds, and games played to predict all star status. This model yeilded a high accuracy in predicting all star status, but when taking a closer look there we discovered slight problems.
## Introduction and Data Description:
In this project, we will design an algorithm to most efficiently predict how many wins a team in the National Basketball Association (NBA) will have in a season. We will also design an algorithm to predict if a player is an all-star for a specific season. To determine team wins we will use specific team data that historically correlates to championships. Specifically, we will use data like ORTG (Offensive Rating), where the higher the rating, the better the team's offense, DRTG (Defensive Rating), where the lower the rating, the better the team’s defense, and TO%, the percentage of possesions that end in turnovers for a team . For determining if a player is an all-star, we will use their total points, total rebounds, along with the total minutes they played in a season.
## Method:
In this project, we decided to use multiple linear regression and gradient descent as our two models. We used multiple linear regression on our first goal, which was predicting the amount of wins a team had based off of their stats that season. To be more specific, we looked at three stats in particular: Offensive Rating, Defensive Rating and Turnover percentage. We believed that these three stats are strong indecators of how well a team would play, which directly translates to wins. We would do this by observing already finished seasons, and using the model to predict the wins based off those seasons stats, and then compare at the end to see how accurate the model was. For our second method, we will use the gradient descent model, and create a 3d graph that maps out certain stats. We have chosen to focus on Points, Total Rebounds and Total Minutes Played, as we look to identify All Stars on each NBA team. The idea is to see if our model can take in these three stats, and identify All Star caliber players. With this method, it assumes a linear relationship between our input features and the outputs, which is safe to assume since being an All star heavily correlates to Points, Rebounds and Minutes Played. Some pitfalls may be that the features are not independent or that the relationship is actually non linear. Either of these pitfalls will cause the model to underperform, and not give us the results we are looking for.

## Results:

### Fig 1 (Model 1):
<img width="687" alt="Screenshot 2024-12-06 at 3 49 57 PM" src="https://github.com/user-attachments/assets/8a75320f-f6f4-4aaa-a8e2-b2f5ddccab93">

As can be seen in the above figure, the histogram roughly follows a symmetrical, normal distribution, ideal for a regression model. Due to the majority of the residuals being close to 0, this indicates that our models predictions were quite close to the actual values for most of the data, although at times the observed value was slighly larger than the predicted value.

### Fig 2 (Model 1):
<img width="629" alt="Screenshot 2024-12-06 at 4 13 16 PM" src="https://github.com/user-attachments/assets/e4606a74-fb37-4b99-9f65-296f65931ce7">

As can be seen in the above figure, there are no clear outliers in the residuals, and they generally cluster closer to 0. Along with this, we see no uniform pattern in the plot of residuals, a good sign for our model. 

## Discussion:
### Model 1
For our first model, we clearly saw that picking ORTG, DRTG, and TO% of a team were very strong indicators of how many wins a team had. For example, our ML model correctly predicted the 2024 Boston Celtics, who won the championship, to be the best team, and predicted the 2016 Philadelphia 76ers (who had a record of 10 wins to 72 losses) to be the worst team. Furthermore, our ML model generated an R^2 of 0.8958476288965742, showing that our ML model is quite accurate in predicting the actual data.Our ML model also generated an MSE of 14.706814990817946, which shows that there is a low variance in errors in our ML model. Although our model is quite accurate, it is not perfect. Thus, you could take it's predictions at face value, but they might not always be correct. Due to this, we might want to see if any other team analytics correlate more to the success of a team, and add that analytic to our model to make it more accurate. Something that arose from our work, is that we noticed that two seasons (2020 and 2021) were shortened due to COVID, so we had to figure out how to navigate through this, as teams had less wins and losses because they played less games. To ensure the number of games didn't matter, we could have had our model instead predict team win percentage instead of total wins. Lastly, we determined that this model does not have any ethical concerns, as there is no moral or physical harm that is raised from predicting the number of wins of a team (unless it hurts the teams feelings). 
### Model 2
For our second model, we saw that using a players total points, total rebounds, and total minutes played poised to be very accurate in predicting if a player made an All-Star team that season. After 1000 iterations, our model had an accuracy of 97%, clearly showing our model was able to answer our question of being able to predict if a player was an All-Star. With this accuracy, we can accept these results at face value, although some assumptions can rarely be incorrect. With such a high accuracy, we likely do not have to change any of the data points we used, as the 3% inaccuracy could be due to injuries during the All-Star game. On the same topic, while working we noticed that this was a concern we had, and in the future we would have to find a way to not include players that missed the All-Star game due to injury in our learning dataset to make our model more accurate. For our model, ethically, it should not be used by the NBA to actually determine what players make or miss the All-Star game, as in the real world, there are a lot more things that go in to a player making the All-Star team than only the data we used, so some players may wrongfully miss the All-Star game with our model.
