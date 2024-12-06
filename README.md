# Final Report
## Abstract:

## Introduction and Data Description:
In this project, we will design an algorithm to most efficiently predict which team in the National Basketball Association (NBA) will win the championship. Along with this, our algorithm will be able to identify and select specific players who are upcoming free agents (players with no contract with any team), and match them to a team who needs their skillset the most. In other words, our algorithm will select available players to join a team to maximize that team's chance to win a championship, based on its belief of what makes a team most likely to win a championship. To determine what teams have the best chance of winning a championship, we will use specific team data that historically correlates to championships. Specifically, we will use data like ORTG (Offensive Rating), where the higher the rating, the better the team's offense, and DRTG (Defensive Rating), where the lower the rating, the better the team’s defense. For example, last year, the Boston Celtics won the NBA championship. The Celtics ranked 1st in ORTG (123.2) and 3rd in DRTG (111.6) of all thirty NBA teams. In fact, the Celtics were the only NBA team to be top 3 in both. Other data that may be helpful to determine the NBA team most likely to win a championship is TS% (True shooting percentage [A players averaged shooting percentage between 2 point shots, 3 point shots, and 1 point shots]), which the Celtics also ranked 1st in. Average team age may be helpful as well, as only one team in NBA history has won a championship with an average age of 26.5 or below (age calculated by [sum of age * minutes] / [ sum of minutes]). Similarly, for determining what player (that is a free agent) best optimizes a team to win a championship, we will use the same data, but at an individual level. (ORTG, DRTG, TS%, Age) all exist as individual stats for players as well. Thus, if a team has a top DRTG, but lacks in ORTG, our algorithm will likely assign a player with a high ORTG to join that team, to maximize their chance of winning a championship. 


## Method:

## Results:

## Discussion:
